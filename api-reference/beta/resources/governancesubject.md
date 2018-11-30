---
title: tipo de recurso de governanceSubject
description: Representa os usuários, grupos e entidades de serviço estão sendo gerenciadas no gerenciamento de identidade privilegiado (PIM).
ms.openlocfilehash: c2129a0da488d4e7f425d6ef3596a955269e0da8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033767"
---
# <a name="governancesubject-resource-type"></a>tipo de recurso de governanceSubject

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa os usuários, grupos e entidades de serviço estão sendo gerenciadas no gerenciamento de identidade privilegiado (PIM).


## <a name="properties"></a>Propriedades
| Propriedade  | Tipo       |Descrição|
|:----------|:----------|:----------|
|id         |String     | A identificação do assunto.|
|type       |String     |O tipo do assunto. O valor pode ser ``User``, ``Group``, e ``ServicePrincipal``.|
|displayName|String     |O nome de exibição do assunto.|
|email      |String     |O endereço de email da entidade do usuário. Se o assunto estiver em outros tipos, está vazio.|
|principalName|Cadeia de caracteres   |O nome principal da entidade do usuário. Se o assunto estiver em outros tipos, está vazio.|

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->