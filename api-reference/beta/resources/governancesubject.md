---
title: Tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço que estão sendo gerenciadas Privileged Identity Management (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: c3e37d9391bedba160c67f6c30e2f386a1524a9f
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454231"
---
# <a name="governancesubject-resource-type"></a>Tipo de recurso governanceSubject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários, grupos e entidades de serviço que estão sendo gerenciadas Privileged Identity Management (PIM).


## <a name="properties"></a>Propriedades
| Propriedade  | Tipo       |Descrição|
|:----------|:----------|:----------|
|id         |Cadeia de caracteres     | A id do assunto.|
|type       |Cadeia de caracteres     |O tipo do assunto. O valor pode ``User`` ser ``Group`` , e ``ServicePrincipal`` .|
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


