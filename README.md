# String Format Specifiers in Swift

```
import UIKit

// String Format Specifiers in Swift

let produto    = "Canetas bic" // usar %@ como placeholder de String
let quantidade = 3             // usar %d como placeholder de Int
let preco      = 10.9999       // usar %f, %.2f como placeholder de Double
let satisfacao = 97.0          // usar %% para escapar o caractere % (porcentagem)

let string1 = String(format: "Sua compra: %d | %@ | preço unitário: R$%.2f | total: R$%.2f", quantidade, produto, preco, preco * Double(quantidade) )
let string2 = String(format: "Esse produto tem um índice de satisfação de %.2f%%", satisfacao )

print(string1)
print(string2)

// Sua compra: 3 | Canetas bic | preço unitário: R$11.00 | total: R$33.00
// Esse produto tem um índice de satisfação de 97.00%
```
