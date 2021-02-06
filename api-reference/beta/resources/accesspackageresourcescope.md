---
title: Tipo de recurso accessPackageResourceScope
description: No gerenciamento de direitos do Azure AD, um escopo de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1491028bb566e8742dcfc1e4928681f61e5272c7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133585"
---
# <a name="accesspackageresourcescope-resource-type"></a>Tipo de recurso accessPackageResourceScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um escopo de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso, para esses recursos que têm vários escopos.

Você pode determinar o escopo de recurso do pacote de acesso, para um recurso que já foi adicionado a um pacote de acesso, usando a lista [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) para retornar uma coleção de [objetos accessPackageResourceRoleScope.](accesspackageresourcerolescope.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|A descrição do escopo.|
|displayName|String|O nome de exibição do escopo.|
|id|String| Somente leitura.|
|isRootScope|Boolean|True se os escopos são organizados em uma hierarquia e este é o escopo superior ou raiz do recurso.|
|originId|String|O identificador exclusivo do escopo no recurso, conforme definido no sistema de origem.|
|originSystem|String|O sistema de origem do escopo.|
|roleOriginId|String|O sistema de origem para a função, se diferente.|
|url|Cadeia de caracteres|Um localizador de recursos para o escopo.|

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
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isRootScope": true,
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


