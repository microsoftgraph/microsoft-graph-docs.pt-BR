---
title: Tipo de recurso educationRoot
description: 'O namespace `/education` expõe funcionalidade específica ao setor de educação. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f93b35dc48087b8d40db0cc3eabc2ba3ba10c8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032681"
---
# <a name="educationroot-resource-type"></a>Tipo de recurso educationRoot

Namespace: microsoft.graph

O namespace `/education` expõe funcionalidade específica ao setor de educação. Alguns objetos no namespace `/education` podem ser encontrados em outras partes do Microsoft Graph (por exemplo, [usuários](user.md)). O namespace education fornece propriedades e recursos específicos de educação nesses objetos.

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar educationClass](../api/educationroot-post-classes.md) |[educationClass](educationclass.md)| Crie uma nova **educationClass** postando na coleção de aulas.|
|[Listar classes](../api/educationroot-list-classes.md) |Coleção [educationClass](educationclass.md)| Obtenha uma coleção de objetos **educationClass**.|
|[Criar educationSchool](../api/educationroot-post-schools.md) |[educationSchool](educationschool.md)| Crie uma nova **educationSchool** postando na coleção de escolas.|
|[Listar escolas](../api/educationroot-list-schools.md) |Coleção [educationSchool](educationschool.md)| Obtenha uma coleção de objetos **educationSchool**.|
|[Criar educationUser](../api/educationroot-post-users.md) |[educationUser](educationuser.md)| Crie um novo **educationUser** postando na coleção de usuários.|
|[Listar usuários](../api/educationroot-list-users.md) |Coleção [educationUser](educationuser.md)| Obtenha uma coleção de objetos **educationUser**.|

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classes|Coleção [educationClass](educationclass.md)| Somente leitura. Anulável.|
|me|[educationUser](educationuser.md)| Somente leitura. Anulável.|
|schools|Coleção [educationSchool](educationschool.md)| Somente leitura. Anulável.|
|users|Coleção [educationUser](educationuser.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-education-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
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
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

