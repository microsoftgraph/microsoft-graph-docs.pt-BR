# <a name="update-a-group-setting"></a>Atualizar uma configuração de grupo

Atualize as propriedades de um objeto de configuração de grupo específico.

## <a name="prerequisites"></a>Pré-requisitos

Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*

> Observação: Somente os administradores do locatário têm permissões para executar operações de criação, atualização e exclusão.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->

Atualizar uma configuração específica de grupo ou de locatário como um todo.

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais
| Nome | Descrição |
|:-----------|:-----------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. 

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| values | settingValue | O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores. |

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um código de resposta `204 OK` e um objeto [groupSetting](../resources/groupsetting.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->