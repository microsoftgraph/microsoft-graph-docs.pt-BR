---
title: Tipo de recurso accessPackageResourceScope
description: No gerenciamento de direitos do Azure AD, um escopo de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f403f6b2d7c88d1e24c579578c2c1b872bbbecdf
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651229"
---
# <a name="accesspackageresourcescope-resource-type"></a>Tipo de recurso accessPackageResourceScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-overview.md)um escopo de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso, para esses recursos que têm vários escopos.

Você pode determinar o escopo de recurso do pacote de acesso, para um recurso que já tenha funções adicionadas a um pacote de acesso, usando [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) de lista para retornar uma coleção de objetos [accessPackageResourceRoleScope.](accesspackageresourcerolescope.md)

Se o recurso estiver em um catálogo de pacotes de acesso, mas ainda não tiver suas funções adicionadas a um pacote de acesso, você poderá determinar o escopo de recurso do pacote de acesso usando o [accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md) de lista e incluindo na `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` consulta.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|A descrição do escopo.|
|displayName|String|O nome de exibição do escopo.|
|id|String| Somente leitura.|
|isRootScope|Booliano|True se os escopos são organizados em uma hierarquia e este é o escopo superior ou raiz do recurso.|
|originId|String|O identificador exclusivo do escopo no recurso conforme definido no sistema de origem.|
|originSystem|String|O sistema de origem do escopo.|
|roleOriginId|String|O sistema de origem da função, se diferente.|
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


