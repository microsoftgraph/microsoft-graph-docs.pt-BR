# <a name="update-alert"></a>Update alert

Atualiza uma propriedade editável **alert** dentro de qualquer solução integrada para manter o status do alerta e as tarefas atribuídas em sincronia em todas soluções. Este método atualiza qualquer solução que tenha um registro do alerta referenciado pelo ID.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |   SecurityEvents.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

> **Observação:** Você deve incluir o ID do **alerta** como parâmetro e vendorInformation contendo `provider` e `vendor` neste método.
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Authorization  | Portador {código}. Obrigatório.|
|Prefer | return=representation |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. O corpo **deve** conter a propriedade `vendorInformation` com os campos `provider` e `vendor` válidos. A tabela a seguir lista os campos que podem ser atualizados em um alerta. Os valores para propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados. Para alcançar um melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|assignedTo|Cadeia de caracteres|Nome do analista para quem foi atribuída a triagem, investigação ou correção do alerta.|
|closedDateTime|DateTimeOffset|Hora em que o alerta foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|comments|Coleção de cadeias de caracteres|Comentários do analista sobre o alerta (para gerenciamento de alerta do cliente).|
|feedback|alertFeedback|Feedback do analista sobre o alerta. Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|alertStatus|Status do ciclo de vida do alerta (estágio). Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.|
|tags|Coleção de cadeias de caracteres|Rótulos definidos pelo usuário que podem ser aplicados a um alerta e servir como condições de filtro (por exemplo, "HVA", "SAW").|
|vendorInformation *|[securityVendorInformation](../resources/securityvendorinformation.md)|Tipo complexo contendo detalhes sobre o produto de segurança/provedor de serviço (por exemplo, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker). **Os campos provider e vendor são obrigatórios.**|
(\* Indica um campo obrigatório.)

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Se o cabeçalho opcional da solicitação for usado, o método retornará um código de resposta `200 OK` e o objeto [alert](../resources/alert.md) atualizado no corpo da resposta.

## <a name="example-1"></a>Exemplo 1

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>Resposta

Este é um exemplo de uma resposta bem-sucedida.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a>Exemplo 2

### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação que inclui o cabeçalho de solicitação `Prefer`.

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

### <a name="response"></a>Resposta

A seguir está um exemplo da resposta quando o cabeçalho de solicitação opcional `Prefer: return=representation` é usado.

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
