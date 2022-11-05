# Funcoes1

 /* 
1- Débito
2- Dinheiro ou PIX
3- Parcelado 2x
3- Parcelado 3x ou mais
*/
function aplicarDesconto (valor, desconto) {
    return (valor - (valor * (desconto / 100)));
}

function aplicarJuros (valor, juros) {
    return (valor + (valor * (juros / 100)));
}
const precoEtiqueta = 500;
const formaPagamento = 4;

if (formaPagamento === 1) {
    console.log(aplicarDesconto(precoEtiqueta, 10));
} else if (formaPagamento === 2) {
    console.log(aplicarDesconto(precoEtiqueta, 15));
} else if (formaPagamento === 3) {
    console.log(aplicarDesconto(precoEtiqueta, 0));
} else if (formaPagamento === 4) {
    console.log(aplicarJuros(precoEtiqueta, 10));
}
