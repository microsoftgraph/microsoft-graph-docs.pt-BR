---
title: Tipo de recurso governanceSubject
description: Representa usuários, grupos e entidades de serviço sendo gerenciadas no Privileged Identity Management (PIM).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: eedcaff8538d5a0efa110b34cd6a72aef2a3210a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132663"
---
# <a name="governancesubject-resource-type"></a>Tipo de recurso governanceSubject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa usuários, grupos e entidades de serviço sendo gerenciadas no Privileged Identity Management (PIM).


## <a name="properties"></a>Propriedades
| Propriedade  | Tipo       |Descrição|
|:----------|:----------|:----------|
|id         |String     | A id do assunto.|
|type       |String     |O tipo do assunto. O valor pode ser ``User`` ``Group`` , e ``ServicePrincipal`` .|
|displayName|String     |O nome de exibição do assunto.|
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


