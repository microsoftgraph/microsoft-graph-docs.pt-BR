---
title: Tipo de recurso accessPackageResourceRoleScope
description: Um escopo de função de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso e a uma função nesse recurso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1a70240029f42b5a746d293bc8939f669b651240
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651236"
---
# <a name="accesspackageresourcerolescope-resource-type"></a>Tipo de recurso accessPackageResourceRoleScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-overview.md)um escopo de função de recurso do pacote de acesso é uma referência a um escopo dentro de um recurso e uma função nesse recurso para esse escopo.  Um pacote de acesso terá escopos de função de recurso de pacote de acesso para os recursos em seu catálogo que são relevantes para esse pacote de acesso.  Quando um assunto recebe uma atribuição de pacote de acesso, o assunto será provisionado com a função nesse escopo de cada escopo de função de recurso do pacote de acesso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md) | Recupere uma lista de **objetos accessPackageResourceRoleScope** para um pacote de acesso. |
| [Criar accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Crie um novo **objeto accessPackageResourceRoleScope** para um pacote de acesso. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdBy|String|Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|id|String| Somente leitura.|
|modifiedBy|String|Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| Somente leitura. Anulável. Suporta o `$expand`.|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "keyProperty": "id"
}-->

```json
{
   "createdBy":"String",
   "createdDateTime":"String (timestamp)",
   "id":"String (identifier)",
   "modifiedBy":"String",
   "modifiedDateTime":"String (timestamp)",
   "accessPackageResourceRole":{
      "id":"String (identifier)",
      "displayName":"String",
      "originSystem":"String",
      "originId":"String"
   },
   "accessPackageResourceScope":{
      "id":"String (identifier)",
      "displayName":"String",
      "description":"String",
      "originId":"String (identifier)",
      "originSystem":"String"
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


