---
title: Tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço que estão sendo gerenciadas Privileged Identity Management (PIM).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 99e668cc18ff38f8a4b26c11d514beddcc020e00
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509634"
---
# <a name="governancesubject-resource-type"></a>Tipo de recurso governanceSubject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários, grupos e entidades de serviço que estão sendo gerenciadas Privileged Identity Management (PIM).


## <a name="properties"></a>Propriedades
| Propriedade  | Tipo       |Descrição|
|:----------|:----------|:----------|
|id         |Cadeia de caracteres     | A id do assunto.|
|type       |String     |O tipo do assunto. O valor pode ser ``User``, ``Group``e ``ServicePrincipal``.|
|displayName|Cadeia de caracteres     |O nome de exibição do assunto.|
|email      |Cadeia de caracteres     |O endereço de email do assunto do usuário. Se o assunto estiver em outros tipos, ele está vazio.|
|principalName|Cadeia de caracteres   |O nome principal do assunto do usuário. Se o assunto estiver em outros tipos, ele está vazio.|

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


