---
title: tipo de recurso de governanceSubject
description: Representa os usuários, grupos e entidades de serviço estão sendo gerenciadas no gerenciamento de identidade privilegiado (PIM).
localization_priority: Normal
ms.openlocfilehash: f3f8762c9136a3ae92269f6c06f52000fb73f710
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832587"
---
# <a name="governancesubject-resource-type"></a>tipo de recurso de governanceSubject

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa os usuários, grupos e entidades de serviço estão sendo gerenciadas no gerenciamento de identidade privilegiado (PIM).


## <a name="properties"></a>Propriedades
| Propriedade  | Tipo       |Descrição|
|:----------|:----------|:----------|
|id         |Cadeia de caracteres     | A identificação do assunto.|
|type       |Cadeia de caracteres     |O tipo do assunto. O valor pode ser ``User``, ``Group``, e ``ServicePrincipal``.|
|displayName|Cadeia de caracteres     |O nome de exibição do assunto.|
|email      |Cadeia de caracteres     |O endereço de email da entidade do usuário. Se o assunto estiver em outros tipos, está vazio.|
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
