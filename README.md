# javascript-test-0002-final-15968-nisha
Final Project Assignment - This repository contains the complete final project code and documentation.
function factorial(n) {
    let f = 1;
    for (let i = 1; i <= n; i++) {
        f = f * i;
    }
    return f;
}

function nCr(n, r) {
    return factorial(n) / (factorial(r) * factorial(n - r));
}

let n = 5;

for (let i = n - 1; i >= 0; i--) {

    
    for (let s = 0; s < n - 1 - i; s++) {
        process.stdout.write(" ");
    }

    
    for (let j = 0; j <= i; j++) {
        process.stdout.write(nCr(i, j) + " ");
    }

    console.log();
}
