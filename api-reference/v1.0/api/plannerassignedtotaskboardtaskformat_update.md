# <a name="update-plannerassignedtotaskboardtaskformat"></a>Atualizar plannerAssignedToTaskBoardTaskFormat

Atualize as propriedades do objeto **plannerAssignedToTaskBoardTaskFormat**.
### <a name="prerequisites"></a>Pré-requisitos
Os seguintes **escopos** são necessários para executar esta API: 

*Group.ReadWrite.All*

### <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/assignedToTaskBoardFormat
```
### <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | <code> de portador|
| If-Match  | Último valor ETag conhecido do objeto **plannerAssignedToTaskBoardTaskFormat** a ser atualizado. Obrigatório.|

### <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](..\resources\plannerOrderHintsByAssignee.md)|O dicionário de dicas usado para ordenar tarefas no modo de exibição AssignedTo do Quadro de Tarefas. A chave de cada entrada é um dos usuários ao qual a tarefa é atribuída, e o valor é a dica de ordem. O formato de cada valor é definido como descrito [aqui](../resources/planner_order_hint_format.md).|
|unassignedOrderHint|String|Valor da dica usado para ordenar a tarefa no modo de exibição AssignedTo do Quadro de Tarefas quando a tarefa não for atribuída a ninguém ou se o dicionário orderHintsByAssignee não oferecer uma dica de ordem para o usuário à qual a tarefa foi atribuída. O formato é definido como descrito [aqui](../resources/planner_order_hint_format.md).|

### <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) atualizado no corpo da resposta.

Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).

### <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_plannerassignedtotaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat
Content-type: application/json
Content-length: 96
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHintsByAssignee": {
    "aaa27244-1db4-476a-a5cb-004607466324": "8566473P 957764Jk!"
  }
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerassignedtotaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->