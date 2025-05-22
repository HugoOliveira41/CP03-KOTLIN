# CP3-ANDROID — Aplicativo de Lista de Compras em Kotlin

Aplicativo Android desenvolvido em Kotlin que permite ao usuário cadastrar, visualizar, editar e excluir itens de uma lista de compras de maneira simples e intuitiva.

## Organização dos Arquivos Kotlin

### MainActivity.kt
Este é o núcleo da interface do app.

- Responsável por exibir os produtos utilizando uma RecyclerView.
- Gerencia as interações: adição, edição e remoção de produtos.
- Realiza a comunicação com a Service.kt para obter os dados atualizados.
- Atua como controlador da tela principal: ouve os eventos, processa as ações e reflete as mudanças em tempo real.

### Model.kt
Arquivo que define o modelo de dados do app, ou seja, a estrutura da classe Produto.

Cada produto contém:

- id: identificador único de cada item (como o RG do produto).
- nome: descrição do item da compra (como leite, pão, margarina...).
- quantidade: número de unidades desejadas.

### Service.kt
Contém toda a lógica de manipulação dos dados da lista de compras:

- Insere novos produtos na lista.
- Remove itens existentes.
- Atualiza informações de um produto.
- Fornece o conjunto completo de itens cadastrados.

### Factory.kt
Controla a criação e reaproveitamento do serviço ProdutoService.

- Garante que apenas uma instância seja utilizada sempre que possível.
- Evita a criação desnecessária de objetos, otimizando o desempenho.

## Demonstração

- Imagens do app em funcionamento no emulador Android.
- Exibição do código-fonte correspondente à execução.

---

**HUGO ANTONIO DE OLIVEIRA**  
**RM: 550153**

