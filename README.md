# Estrutura de Dados - DHT
 Ponderada de prog feita por Marcelo Rubim Rossignolli

### **Caso de Teste 1: Inserção de um Novo Par Chave-Valor**
- **Pré-condição:** A DHT está inicializada e pelo menos um nó está ativo.
- **Etapas do Teste:**
  1. Criar um par chave-valor (exemplo: chave = `"user123"`, valor = `"dataXYZ"`).
  2. Inserir a chave-valor na DHT.
  3. Verificar se a chave-valor foi armazenada corretamente consultando a DHT.
- **Pós-condição:** A chave-valor está presente na DHT e pode ser recuperada posteriormente.

---

### **Caso de Teste 2: Recuperação de um Valor Existente**
- **Pré-condição:** A chave-valor a ser consultada já foi inserida na DHT.
- **Etapas do Teste:**
  1. Enviar uma requisição para recuperar o valor correspondente a uma chave conhecida.
  2. Verificar se a resposta contém o valor correto associado à chave.
- **Pós-condição:** O valor correto é retornado e exibido sem erros.

---

### **Caso de Teste 3: Remoção de um Par Chave-Valor**
- **Pré-condição:** A chave-valor já está presente na DHT.
- **Etapas do Teste:**
  1. Enviar uma requisição para remover a chave-valor da DHT.
  2. Tentar recuperar o valor correspondente à chave removida.
  3. Verificar se a chave não pode mais ser encontrada.
- **Pós-condição:** A chave-valor foi removida com sucesso e não pode mais ser recuperada.

---

### **Caso de Teste 4: Rebalanceamento após a Entrada de um Novo Nó**
- **Pré-condição:** A DHT está funcional e contém pelo menos dois nós ativos.
- **Etapas do Teste:**
  1. Adicionar um novo nó à rede DHT.
  2. Verificar se a redistribuição das chaves ocorre corretamente.
  3. Consultar algumas chaves para garantir que estão sendo direcionadas para os nós corretos.
- **Pós-condição:** O novo nó está integrado e as chaves foram redistribuídas corretamente.

---

### **Caso de Teste 5: Recuperação após a Falha de um Nó**
- **Pré-condição:** A DHT possui pelo menos três nós e está operando normalmente.
- **Etapas do Teste:**
  1. Desativar um nó contendo chaves armazenadas.
  2. Tentar recuperar as chaves que estavam armazenadas nesse nó.
  3. Verificar se os dados foram recuperados corretamente de um nó redundante.
- **Pós-condição:** A DHT recupera os dados corretamente utilizando mecanismos de replicação ou redistribuição.