const test = require('tape')
const index = require ('./atividade')
const {quantidadeDePares, quadrado, calcularAreaRetangulo} = require("./atividade")

test("teste pares - 1", (t) => {
    t.assert(
        quantidadeDePares([1, 2, 3]) === 1,
        "Calculou corretamente"
    )
    t.end()
})
test("teste pares - 2", (t) => {
    t.assert(
        quantidadeDePares([]) === 0,
        "Calculou corretamente"
    )
    t.end()
})
test("teste pares - 3", (t) => {
    t.assert(
        quantidadeDePares([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]) === 5,
        "Calculou corretamente"
    )
    t.end()
})

test("teste ao quadrado - 1", (t) => {
    t.assert(
        quadrado(2) === 4,
        "Calculou corretamente"
    )
    t.end()
})
test("teste ao quadrado - 2", (t) => {
    t.assert(
        quadrado(10) === 100,
        "Calculou corretamente"
    )
    t.end()
})
test("teste ao quadrado - 3", (t) => {
    t.assert(
        quadrado(32) === 1024,
        "Calculou corretamente"
    )
    t.end()
})

test("teste área - 1", (t) => {
    t.assert(
        calcularAreaRetangulo(10, 50) === 500,
        "Calculou corretamente"
    )
    t.end()
})
test("teste área - 2", (t) => {
    t.assert(
        calcularAreaRetangulo(2, 2) === 4,
        "Calculou corretamente"
    )
    t.end()
})
test("teste área - 3", (t) => {
    t.assert(
        calcularAreaRetangulo(58, 32) === 1856,
        "Calculou corretamente"
    )
    t.end()
})