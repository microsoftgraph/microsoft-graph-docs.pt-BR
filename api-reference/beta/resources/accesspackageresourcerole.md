---
title: tipo de recurso accessPackageResourceRole
description: Uma referência a uma função definida em um Resource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b5ab0cc6e2179adb62316cbcdc06b7dd52abc439
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508510"
---
# <a name="accesspackageresourcerole-resource-type"></a>tipo de recurso accessPackageResourceRole

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de pacote do Access é uma referência a uma função definida em um recurso, que pode ser usada em um pacote do Access.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | coleção [accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de objetos accessPackageResourceRole para um catálogo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Uma descrição para a função de recurso.|
|displayName|Cadeia de caracteres|O nome de exibição da função de recurso como a função definida pelo aplicativo.|
|id|String| Somente leitura.|
|originid|String|O identificador exclusivo da função de recurso no sistema de origem. |
|originSystem|String|O tipo do recurso no sistema de origem.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
