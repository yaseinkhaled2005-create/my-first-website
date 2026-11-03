
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="الوزير كلاسك - ملك الشطرنج، فلسفة العقل والتخطيط والاستراتيجية">
<title>الوزير كلاسك | ملك الشطرنج</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    background: #111111;
    color: #eee4cf;
    font-family: Tahoma, Arial, sans-serif;
    text-align: center;
}

header {
    padding: 35px 15px 20px;
    background: linear-gradient(180deg, #24211b, #111111);
    border-bottom: 1px solid #92743c;
}

.crown {
    font-size: 38px;
    color: #d5b46b;
}

h1 {
    color: #d5b46b;
    font-size: 34px;
    margin: 12px 0;
    letter-spacing: 2px;
}

.subtitle {
    color: #f0dfb5;
    font-size: 19px;
    letter-spacing: 3px;
}

.english {
    color: #aa9569;
    font-size: 13px;
    margin-top: 15px;
    direction: ltr;
}

section {
    max-width: 750px;
    margin: 30px auto;
    padding: 20px;
}

h2 {
    color: #d5b46b;
    font-size: 23px;
    margin-bottom: 20px;
}

.quote {
    color: #c9c0b0;
    line-height: 2.2;
    font-size: 17px;
    padding: 15px;
    border-top: 1px solid #66532f;
    border-bottom: 1px solid #66532f;
}

.gold {
    color: #d5b46b;
}

.board-wrap {
    max-width: 470px;
    margin: 25px auto;
    padding: 10px;
    border: 2px solid #a88a4d;
    border-radius: 5px;
    background: #29251d;
    direction: ltr;
}

.board {
    display: grid;
    grid-template-columns: repeat(8, 1fr);
    width: 100%;
    aspect-ratio: 1;
}

.square {
    border: none;
    border-radius: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    cursor: pointer;
    aspect-ratio: 1;
    font-size: clamp(23px, 7vw, 46px);
    line-height: 1;
}

.light {
    background: #e5d2aa;
}

.dark {
    background: #806343;
}

.square.selected {
    background: #c5a34c;
}

.square.hint::after {
    content: "";
    position: absolute;
    width: 24%;
    height: 24%;
    background: #294e31;
    border-radius: 50%;
    opacity: .8;
}

.square.capture::after {
    content: "";
    position: absolute;
    inset: 3px;
    border: 4px solid #294e31;
    border-radius: 50%;
}

.white-piece {
    color: #fffdf3;
    text-shadow: 1px 2px 2px #292929;
}

.black-piece {
    color: #17130f;
    text-shadow: 0 1px 1px #e0c99b;
}

.controls {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 10px;
    margin: 20px 0;
}

button.control {
    padding: 12px 22px;
    background: #29251d;
    color: #d5b46b;
    border: 1px solid #a88a4d;
    border-radius: 4px;
    cursor: pointer;
    font-size: 15px;
}

button.control:hover {
    background: #514127;
}

.status {
    color: #d5b46b;
    min-height: 30px;
    margin: 15px;
}

.moves {
    color: #d6c9ad;
    direction: ltr;
    text-align: left;
    line-height: 2;
    max-height: 120px;
    overflow-y: auto;
    font-size: 14px;
}

footer {
    margin-top: 45px;
    padding: 25px 10px;
    border-top: 1px solid #92743c;
    color: #aa9569;
    font-size: 13px;
}

@media(max-width: 480px) {
    h1 { font-size: 27px; }
    section { padding: 12px; }
    .quote { font-size: 15px; }
}
</style>
</head>

<body>

<header>
    <div class="crown">♛</div>
    <h1>الوزير كلاسك</h1>
    <div class="subtitle">مَلِكُ الشَّطْرَنْج</div>
    <div class="english">THE MINISTER CLASSIC</div>
</header>

<section>
    <h2>فلسفة العقل والاستراتيجية</h2>

    <div class="quote">
        ليس كل من امتلك القطع أتقن اللعبة،
        وليس كل من خسر جولة فقد المعركة.
        <br>
        <span class="gold">
            العقل يسبق الحركة، والبصيرة تصنع الانتصار.
        </span>
    </div>
</section>

<section>
    <h2>رقعة الملوك</h2>

    <p class="quote">
        لكل قطعة دور، ولكل حركة غاية.
        اختر قطعتك وابدأ اللعب.
    </p>

    <div class="board-wrap">
        <div class="board" id="board"></div>
    </div>

    <div class="status" id="status">
        الأبيض يبدأ اللعب
    </div>

    <div class="controls">
        <button class="control" id="undo">تراجع</button>
        <button class="control" id="restart">إعادة اللعبة</button>
    </div>

    <h2>سجل الحركات</h2>
    <div class="moves" id="moves">لم تبدأ اللعبة بعد.</div>
</section>

<section>
    <h2>قانون الملك</h2>
    <div class="quote">
        القوة ليست في عدد القطع،
        بل في كيفية استخدامها.
        <br><br>
        لا تتحرك بلا هدف،
        ولا تكشف خطتك قبل أوانها.
        <br><br>
        <span class="gold">فالعقل سيد الرقعة.</span>
    </div>
</section>

<footer>
    <div class="gold">♛ الوزير كلاسك ♛</div>
    <p>YASSIN | THE CHESS MIND</p>
    <p>© 2026 جميع الحقوق محفوظة</p>
</footer>

<script type="module">
import { Chess } from
"https://esm.sh/chess.js@1.0.0";

const game = new Chess();

const board = document.getElementById("board");
const status = document.getElementById("status");
const moves = document.getElementById("moves");

let selected = null;
let possible = [];

const pieces = {
    wk:"♔", wq:"♕", wr:"♖",
    wb:"♗", wn:"♘", wp:"♙",
    bk:"♚", bq:"♛", br:"♜",
    bb:"♝", bn:"♞", bp:"♟"
};

function drawBoard() {
    board.innerHTML = "";

    const position = game.board();

    for (let r = 0; r < 8; r++) {
        for (let c = 0; c < 8; c++) {

            const square = document.createElement("button");
            square.className =
                "square " + ((r+c)%2===0 ? "light":"dark");

            square.type = "button";

            const file = "abcdefgh"[c];
            const rank = 8-r;
            const name = file + rank;

            const piece = position[r][c];

            if (piece) {
                const color =
                    piece.color === "w" ? "w" : "b";

                square.textContent =
                    pieces[color + piece.type];

                square.classList.add(
                    piece.color === "w"
                    ? "white-piece"
                    : "black-piece"
                );
            }

            if (selected === name) {
                square.classList.add("selected");
            }

            const target = possible.find(m => m.to === name);

            if (target) {
                square.classList.add(
                    piece ? "capture" : "hint"
                );
            }

            square.addEventListener("click", () => {
                chooseSquare(name);
            });

            board.appendChild(square);
        }
    }

    updateStatus();
    updateMoves();
}

function chooseSquare(name) {

    if (selected === null) {

        const piece = game.get(name);

        if (!piece || piece.color !== game.turn()) {
            return;
        }

        selected = name;

        possible = game.moves({
            square: name,
            verbose: true
        });

        drawBoard();
        return;
    }

    if (selected === name) {
        selected = null;
        possible = [];
        drawBoard();
        return;
    }

    try {
        const move = game.move({
            from: selected,
            to: name,
            promotion: "q"
        });

        if (move) {
            selected = null;
            possible = [];
            drawBoard();
            return;
        }
    } catch (e) {}

    const piece = game.get(name);

    if (piece && piece.color === game.turn()) {
        selected = name;

        possible = game.moves({
            square: name,
            verbose: true
        });
    } else {
        selected = null;
        possible = [];
    }

    drawBoard();
}

function updateStatus() {

    if (game.isCheckmate()) {
        status.textContent =
            "انتهت اللعبة بالكش مات! الفائز: " +
            (game.turn() === "w" ? "الأسود" : "الأبيض");
    } else if (game.isDraw()) {
        status.textContent = "انتهت اللعبة بالتعادل.";
    } else {
        status.textContent =
            (game.turn() === "w" ? "دور الأبيض" : "دور الأسود") +
            (game.isCheck() ? " — كش!" : "");
    }
}

function updateMoves() {

    const history = game.history();

    if (!history.length) {
        moves.textContent = "لم تبدأ اللعبة بعد.";
        return;
    }

    let output = "";

    for (let i = 0; i < history.length; i += 2) {
        output +=
            (Math.floor(i/2)+1) + ". " +
            history[i] + " " +
            (history[i+1] || "") + "     ";
    }

    moves.textContent = output;
}

document.getElementById("restart")
.addEventListener("click", () => {
    game.reset();
    selected = null;
    possible = [];
    drawBoard();
});

document.getElementById("undo")
.addEventListener("click", () => {
    game.undo();
    selected = null;
    possible = [];
    drawBoard();
});

drawBoard();
</script>

</body>
</html>
