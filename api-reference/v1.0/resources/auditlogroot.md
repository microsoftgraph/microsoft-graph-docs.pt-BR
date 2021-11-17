---
title: Tipo de recurso auditLogRoot
description: Contém diferentes tipos de logs de auditoria. Esses recursos retornam um recurso singleton auditLog. Ele não contém propriedades usáveis.
author: dhanyahk
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0443ab5287dbe8123d88f0f497ea3a5db919939c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015823"
---
# <a name="auditlogroot-resource-type"></a>Tipo de recurso auditLogRoot

Namespace: microsoft.graph

Contém diferentes tipos de logs de auditoria. Esses recursos retornam um recurso singleton auditLog. Ele não contém propriedades usáveis.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |Liste os itens de auditoria de diretório no conjunto de suas propriedades.|
|[Obter directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |Obter um item de auditoria do diretório específico e suas propriedades.|
|[Listar entrar](../api/signin-list.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de objetos de domínio.|
|[Obter entrar](../api/signin-get.md) | [signIn](signin.md) |Leia as propriedades e os relacionamentos de um objeto de domínio.|

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|directoryAudits|[Coleção directoryAudit](directoryaudit.md)| Somente leitura. Anulável.|
|signIns|[Coleção signIn](signin.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.auditLogRoot"
}-->

```json
{
}
```

## <a name="example"></a>Exemplo


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-auditlogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-auditlogs-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditLogRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

