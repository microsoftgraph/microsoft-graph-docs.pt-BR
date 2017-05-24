# <a name="update-plannerprogresstaskboardtaskformat"></a>Atualizar plannerProgressTaskBoardTaskFormat

Atualize as propriedades do objeto **plannerProgressTaskBoardTaskFormat**.
### <a name="prerequisites"></a>Pré-requisitos
Os seguintes **escopos** são necessários para executar esta API: 

*Group.ReadWrite.All*
### <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/progressTaskBoardFormat
```
### <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | <code> de portador|
| If-Match  | Último valor ETag conhecido do objeto **plannerProgressTaskBoardTaskFormat** a ser atualizado. Obrigatório.|

### <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|orderHint|String|Valor da dica usado para ordenar a tarefa no modo de exibição Progress do Quadro de Tarefas. O formato é definido como descrito [aqui](../resources/planner_order_hint_format.md).|

### <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) atualizado no corpo da resposta.

Este método pode retornar qualquer um dos [códigos de status de HTTP](../../../concepts/errors.md). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner_overview.md#common-planner-error-conditions).

### <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/progressTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update plannerprogresstaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->