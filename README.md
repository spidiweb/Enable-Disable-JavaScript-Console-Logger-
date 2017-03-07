# Enable-Disable-JavaScript-Console-Logger-

//Enable / Disable console.log
var devEnv = true;

var actualConsoleLogger = console.log;

console.log = function () {
    if (devEnv) {
        actualConsoleLogger(arguments);
    }
}
