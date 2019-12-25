---
title: tipo de recurso accessPackageResourceRoleScope
description: Um escopo de função de recurso de pacote do Access é uma referência a um escopo dentro de um recurso e uma função nesse recurso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4ee4ec63c9c2efb60850ee7915e62dc0e284f8ba
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870957"
---
# <a name="accesspackageresourcerolescope-resource-type"></a>tipo de recurso accessPackageResourceRoleScope

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), um escopo de função de recurso de pacote de acesso é uma referência a um escopo dentro de um recurso e uma função nesse recurso para esse escopo.  Um pacote de acesso terá escopos de função de recurso pacote de acesso para os recursos em seu catálogo que são relevantes para esse pacote de acesso.  Quando um assunto recebe uma atribuição de pacote do Access, o assunto será provisionado com a função nesse escopo de cada escopo de função de recurso de pacote de acesso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de objetos **accessPackageResourceRoleScope** para um pacote do Access. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Criar um novo objeto **accessPackageResourceRoleScope** para um pacote do Access. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy|String|Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura.|
|modifiedBy|String|Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| Somente leitura. Anulável.|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "accessPackageResourceRole": {
    "id": "String (identifier)",
     "displayName": "String",
     "originSystem": "String",
     "originId": "String"
  },
  "accessPackageResourceScope": {
     "id": "String (identifier)",
     "displayName": "String",
     "description": "String",
     "originId": "String (identifier)",
     "originSystem": "String"
  }

}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
