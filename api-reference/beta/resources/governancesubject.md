---
title: tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 26f6c6904de97fc96eb1b29b9bcbc376bcf69c61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005972"
---
# <a name="governancesubject-resource-type"></a>tipo de recurso governanceSubject

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários, grupos e entidades de serviço que estão sendo gerenciados no gerenciamento de identidade privilegiada (PIM).


## <a name="properties"></a>Propriedades
| Propriedade  | Tipo       |Descrição|
|:----------|:----------|:----------|
|id         |String     | A ID do assunto.|
|type       |String     |O tipo do assunto. O valor pode ser ``User``, ``Group``e ``ServicePrincipal``.|
|displayName|String     |O nome de exibição do assunto.|
|email      |Cadeia de caracteres     |O endereço de email do assunto do usuário. Se o assunto estiver em outros tipos, ele estará vazio.|
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
