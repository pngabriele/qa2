function quantidadeDePares(lista) {
    let resultado = 0;
    for (const numero of lista) {
        if ((numero % 2) === 0) resultado++
    }

    return resultado
}

function quadrado(numero) {
    return numero ** 2
}

function calcularAreaRetangulo(a, b) {
    return a * b
}

module.exports = {quantidadeDePares, quadrado, calcularAreaRetangulo}


