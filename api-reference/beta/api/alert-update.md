---
title: Atualizar alerta
description: Atualize uma propriedade de alerta editável em qualquer solução integrada para manter o status de alerta e as atribuições em sincronia entre soluções.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: e73af2bb04a7806df0cb09e810f74f310a6f8b98
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942798"
---
# <a name="update-alert"></a>Atualizar alerta

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize uma propriedade **de alerta editável** em qualquer solução integrada para manter o status de alerta e as atribuições em sincronia entre soluções. Este método atualiza qualquer solução que tenha um registro da ID de alerta referenciada.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |   SecurityEvents.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) |  Sem suporte.  |
|Aplicativo | SecurityEvents.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

> **Observação:** Você deve incluir a ID **de** alerta como um parâmetro e vendorInformation contendo `provider` o e com este `vendor` método.
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização  | Portador {código}. Obrigatório.|
|Preferir | return=representation. Opcional. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON dos valores para campos relevantes que devem ser atualizados. O corpo **deve** conter a **propriedade vendorInformation** com campos `provider` `vendor` válidos e válidos. A tabela a seguir lista os campos que podem ser atualizados para um alerta. Os valores das propriedades existentes que não estão incluídas no corpo da solicitação não serão alterados. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|assignedTo|Cadeia de caracteres|Nome do analista ao que o alerta é atribuído para triagem, investigação ou correção.|
|closedDateTime|DateTimeOffset|Tempo em que o alerta foi fechado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|comentários|String collection|Comentários do analista sobre o alerta (para gerenciamento de alertas do cliente). Este método pode atualizar o campo de comentários apenas com os seguintes valores: `Closed in IPC` , `Closed in MCAS` .|
|comentários|alertFeedback enum|Comentários do analista no alerta. Os valores possíveis são: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.|
|status|número alertStatus|Status do ciclo de vida de alerta (estágio). Os valores possíveis são: `unknown`, `newAlert`, `inProgress`, `resolved`.|
|tags|Coleção de cadeias de caracteres|Rótulos definíveis pelo usuário que podem ser aplicados a um alerta e podem servir como condições de filtro (por exemplo, "HVA", "SAW).|
|vendorInformation |[securityVendorInformation](../resources/securityvendorinformation.md)|Tipo complexo que contém detalhes sobre o fornecedor, provedor e subprovedor de produtos / serviços de segurança (por exemplo, fornecedor = Microsoft; provedor = Windows Defender ATP; subProvedor = AppLocker). **Os campos provedor e fornecedor são necessários.**|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

Se o header de solicitação opcional for usado, o método retornará um código de resposta e o objeto `200 OK` [de](../resources/alert.md) alerta atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-request-without-prefer-header"></a>Exemplo 1: Solicitar sem o header Prefer

#### <a name="request"></a>Solicitação

A seguir, um exemplo da solicitação sem `Prefer` o header.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Resposta

Veja a seguir o exemplo de uma resposta bem-sucedida.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Exemplo 2: Solicitar com o header Prefer

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação que inclui o `Prefer` header de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta quando o `Prefer: return=representation` header de solicitação opcional é usado.

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
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


