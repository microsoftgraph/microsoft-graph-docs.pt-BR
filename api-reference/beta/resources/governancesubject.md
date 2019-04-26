---
title: tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).
localization_priority: Normal
ms.openlocfilehash: 5ad4b30abaec66b8ad35835795848645ddd9f17b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333679"
---
# <a name="governancesubject-resource-type"></a>tipo de recurso governanceSubject

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).


## <a name="properties"></a>Propriedades
| Propriedade  | Tipo       |Descrição|
|:----------|:----------|:----------|
|id         |String     | A ID do assunto.|
|tipo       |String     |O tipo do assunto. O valor pode ser ``User``, ``Group``e ``ServicePrincipal``.|
|displayName|String     |O nome de exibição do assunto.|
|email      |String     |O endereço de email do assunto do usuário. Se o assunto estiver em outros tipos, ele estará vazio.|
|principalName|Cadeia de caracteres   |O nome da entidade de segurança do usuário. Se o assunto estiver em outros tipos, ele estará vazio.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
