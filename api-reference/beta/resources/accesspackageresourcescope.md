---
title: tipo de recurso accessPackageResourceScope
description: No gerenciamento de qualificação do Azure AD, um escopo de recurso de pacote do Access é uma referência a um escopo dentro de um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 355838fa9f93cef7d44972b98af317a74036e421
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067521"
---
# <a name="accesspackageresourcescope-resource-type"></a>tipo de recurso accessPackageResourceScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), um escopo de recurso de pacote do Access é uma referência a um escopo dentro de um recurso, para aqueles recursos que têm vários escopos.

Você pode determinar o escopo de recurso do pacote de acesso para um recurso que já tenha sido adicionado a um pacote do Access, usando [list accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) para retornar uma coleção de objetos [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|A descrição do escopo.|
|displayName|Cadeia de caracteres|O nome de exibição do escopo.|
|id|String| Somente leitura.|
|isRootScope|Booliano|True se os escopos são organizados em uma hierarquia e este é o escopo superior ou raiz do recurso.|
|originid|Cadeia de caracteres|O identificador exclusivo do escopo no recurso, conforme definido no sistema de origem.|
|originSystem|Cadeia de caracteres|O sistema de origem para o escopo.|
|roleOriginId|Cadeia de caracteres|O sistema de origem para a função, se for diferente.|
|url|Cadeia de caracteres|Um localizador de recursos para o escopo.|

## <a name="relationships"></a>Relacionamentos

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


