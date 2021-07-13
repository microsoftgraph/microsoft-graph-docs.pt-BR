---
title: Tipo de recurso accessPackageResourceRole
description: Uma referência a uma função definida em um recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1194c27e929a14f738384441ab57f5090d8b1149
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401595"
---
# <a name="accesspackageresourcerole-resource-type"></a>Tipo de recurso accessPackageResourceRole

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma função de recurso do pacote de acesso é uma referência a uma função definida em um recurso. Essa referência pode ser usada após a criação de um pacote de acesso para especificar as funções de cada um dos recursos do catálogo no qual um pacote de acesso deve ser entregue, criando um escopo de função de recurso do pacote de [acesso.](../api/accesspackage-post-accesspackageresourcerolescopes.md)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar funções de recurso accessPackageCatalog](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | [Coleção accessPackageResourceRole](accesspackageresourcerole.md) | Recupere uma lista de objetos accessPackageResourceRole para um catálogo. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|description|Cadeia de caracteres|Uma descrição da função de recurso.|
|displayName|Cadeia de caracteres|O nome de exibição da função de recurso, como a função definida pelo aplicativo.|
|id|String| Somente leitura.|
|originId|Cadeia de caracteres|O identificador exclusivo da função de recurso no sistema de origem. Para um SharePoint online, o originId será o número de sequência da função no site. |
|originSystem|Cadeia de caracteres|O tipo do recurso no sistema de origem, como `SharePointOnline` , `AadApplication` ou `AadGroup` .|

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


