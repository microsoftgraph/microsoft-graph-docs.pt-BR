---
title: Listar alertas
description: Recupere uma lista de objetos Alert.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: d50c3244ae2c0e9f158dc38923136ef3e8656f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459210"
---
# <a name="list-alerts"></a>Listar alertas

Recupere uma lista de objetos [Alert](../resources/alert.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | Escopo securityevents. Read. All, escopo securityevents. ReadWrite. All |

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

Este método oferece suporte aos seguintes [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta:

- `$count`
- `$filter`
- `$orderby`
- `$select`
- `$skip`
- `$top`retornará os principais resultados agregados de cada provedor de API de segurança.  

Para retornar um conjunto de propriedades alternativo, use o `$select` parâmetro de consulta OData para especificar o conjunto de propriedades de **alerta** que você deseja.  Por exemplo, para retornar as propriedades **assignedTo**, **Category**e **Severity** , adicione o seguinte à sua consulta: `$select=assignedTo,category,severity`.

> **Observação:** `$top` tem um limite de 1000 alertas e uma combinação de `$top`  +  `$skip` não pode exceder 6000 alertas. Por exemplo, `/security/alerts?$top=10&$skip=5990` o retornará um `200 OK` código de resposta, `/security/alerts?$top=10&$skip=5991` mas retornará um `400 Bad Request` código de resposta.  Para obter mais informações, consulte [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Authorization  | Portador {código}. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método. O corpo da solicitação será ignorado.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos **Alert** no corpo da resposta. Se um código de status diferente de 2xx ou 404 for retornado de um provedor ou se um provedor expirar, a resposta será um `206 Partial Content` código de status com a resposta do provedor em um cabeçalho de aviso. Para obter mais informações, consulte [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).

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
