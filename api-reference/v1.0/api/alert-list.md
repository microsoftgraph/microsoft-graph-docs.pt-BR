---
title: Listar alertas
description: Recupere uma lista de objetos de alerta.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: d18f49c5e1a0dcc8d079816ff7ad17c6e21df2ee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955027"
---
# <a name="list-alerts"></a>Listar alertas

Recupere uma lista de objetos de [alerta](../resources/alert.md) .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  SecurityEvents.Read.All, SecurityEvents.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | SecurityEvents.Read.All, SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /security/alerts
GET /security/alerts?$top=1
GET /security/alerts?$filter={property} eq '{property-value}'
GET /security/alerts?$filter={property} eq '{property-value}'&$top=5
GET /security/alerts?$filter={property} eq '{property-value}'&{property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método suporta os seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top`retornará os principais resultados agregados de cada provedor de API de segurança.  

Para retornar um conjunto de propriedades alternativo, use o OData `$select` consulta parâmetro para especificar o conjunto de propriedades de **alerta** que você deseja.  Por exemplo, para retornar o **assignedTo**, **categoria**e propriedades de **severidade** , adicione a seguinte à sua consulta: `$select=assignedTo,category,severity`.

> **Observação:** `$top` tem um limite de alertas de 1000 e uma combinação de `$top`  +  `$skip` não pode exceder 6000 alertas. Por exemplo, `/security/alerts?$top=10&$skip=5990` retornará um `200 OK` código de resposta, mas `/security/alerts?$top=10&$skip=5991` retornará um `400 Bad Request` código de resposta.  Para obter mais informações, consulte [respostas de erros de API de segurança do Microsoft Graph](../resources/security-error-codes.md).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização  | Portador {código}. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método. O corpo da solicitação será ignorado.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de **alerta** no corpo da resposta. Se um código de status diferente 2xx ou 404 é retornado por um provedor ou se um provedor de tempo limite, a resposta será um `206 Partial Content` código de status com a resposta do provedor em um cabeçalho de aviso. Para obter mais informações, consulte [respostas de erros de API de segurança do Microsoft Graph](../resources/security-error-codes.md).

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "get_alerts"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/alerts
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "activityGroupName": "activityGroupName-value",
      "assignedTo": "assignedTo-value",
      "azureSubscriptionId": "azureSubscriptionId-value",
      "azureTenantId": "azureTenantId-value",
      "category": "category-value",
      "closedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List alerts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
