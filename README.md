# CourseRate
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Subrate Form</title>

<style>
    body {
        font-family: Arial, sans-serif;
        background: #f2f2f2;
    }

    .rating-box {
        width: 350px;
        margin: 80px auto;
        background: #fff;
        padding: 25px;
        border-radius: 8px;
        text-align: center;
        box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    h2 {
        margin-bottom: 15px;
    }

    .stars {
        direction: rtl;
        display: inline-flex;
    }

    .stars input {
        display: none;
    }

    .stars label {
        font-size: 30px;
        color: #ccc;
        cursor: pointer;
        padding: 5px;
    }

    .stars input:checked ~ label,
    .stars label:hover,
    .stars label:hover ~ label {
        color: gold;
    }

    textarea {
        width: 100%;
        height: 80px;
        margin-top: 15px;
        padding: 8px;
        border-radius: 5px;
        border: 1px solid #ccc;
        resize: none;
    }

    button {
        width: 100%;
        margin-top: 15px;
        padding: 10px;
        background: #28a745;
        color: white;
        border: none;
        border-radius: 5px;
        font-size: 16px;
        cursor: pointer;
    }

    button:hover {
        background: #218838;
    }
</style>
</head>

<body>

<div class="rating-box">
    <h2>Rate Our Course</h2>

    <form>
        <div class="stars">
            <input type="radio" id="star5" name="rate">
            <label for="star5">★</label>

            <input type="radio" id="star4" name="rate">
            <label for="star4">★</label>

            <input type="radio" id="star3" name="rate">
            <label for="star3">★</label>

            <input type="radio" id="star2" name="rate">
            <label for="star2">★</label>

            <input type="radio" id="star1" name="rate">
            <label for="star1">★</label>
        </div>

        <textarea placeholder="Write your feedback..."></textarea>

        <button type="submit">Submit Rating</button>
    </form>
</div>

</body>
</html>
