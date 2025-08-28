# Controle de SKUs e Propriedades

## Editando Requisitos via GitHub

### Estrutura do Arquivo requisitos.json

O arquivo de requisitos fica em `https://github.com/EspanhaFacil/requisitos-json/blob/main/requisitos.json` e segue esta estrutura:

```json
[
  [
    {
      "sku": "CONS-FISC-24665292896",
      "propsDeal": ["quais_sao_as_duvidas_do_cliente_"]
    },
    {
      "sku": "CONS-EDUC-24664410983", 
      "propsDeal": ["qual_curso_o_cliente_tem_interesse_"]
    }
  ],
  [
    {
      "sku": "CURS-CURS-00001469",
      "propsDeal": ["em_qual_curso_o_cliente_tem_interesse_"]
    }
  ]
]
```

### Como Editar pelo GitHub

#### Método 1: Interface Web do GitHub

1. **Acesse o repositório** no GitHub
2. **Navegue até**: `https://github.com/EspanhaFacil/requisitos-json/blob/main/requisitos.json`
3. **Clique no ícone de lápis** (Edit this file) no canto superior direito
4. **Faça suas alterações** seguindo a estrutura JSON
5. **Adicione uma mensagem de commit** descritiva
6. **Clique em "Commit changes"**

### Regras para Edição

#### Estrutura Obrigatória
- **Array de arrays**: O arquivo deve conter um array principal com sub-arrays
- **Objetos de requisito**: Cada item deve ter `sku` (string) e `propsDeal` (array)

#### Exemplo de Adição
```json
{
  "sku": "NOVO-PRODUTO-123",
  "propsDeal": [
    "nova_propriedade_customizada",
    "outra_propriedade_importante"
  ]
}
```
