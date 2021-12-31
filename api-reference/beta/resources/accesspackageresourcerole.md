---
title: Tipo de recurso accessPackageResourceRole
description: Uma referência a uma função definida em um recurso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5652e9c867b235bc87cf67584056ce4425f1da80
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651186"
---
# <a name="accesspackageresourcerole-resource-type"></a>Tipo de recurso accessPackageResourceRole

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-overview.md)uma função de recurso do pacote de acesso é uma referência a uma função definida em um recurso. Essa referência pode ser usada após a criação de um pacote de acesso para especificar as funções de cada um dos recursos do catálogo no qual um pacote de acesso deve ser entregue, criando um escopo de função de recurso do pacote de [acesso.](../api/accesspackage-post-accesspackageresourcerolescopes.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Coleção accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de objetos accessPackageResourceRole para um catálogo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|String|Uma descrição da função de recurso.|
|displayName|String|O nome de exibição da função de recurso, como a função definida pelo aplicativo.|
|id|String| Somente leitura.|
|originId|String|O identificador exclusivo da função de recurso no sistema de origem. Para um SharePoint online, o originId será o número de sequência da função no site. |
|originSystem|String|O tipo do recurso no sistema de origem, como `SharePointOnline` , `AadApplication` ou `AadGroup` .|

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


