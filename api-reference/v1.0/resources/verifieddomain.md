---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade verifiedDomains da entidade da organização é uma coleção de objetos verifiedDomain.
ms.localizationpriority: medium
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 0205971eff906b6c4adb33490bd8e7ea6b3e3a5f
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247242"
---
# <a name="verifieddomain-resource-type"></a>Tipo de recurso verifiedDomain

Namespace: microsoft.graph

Especifica um domínio de um locatário. A **propriedade verifiedDomains** da entidade [da](organization.md) organização é uma coleção de **objetos verifiedDomain** .


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo    | Descrição                                                                          |
|:-------------|:--------|:-------------------------------------------------------------------------------------|
| capabilities | Cadeia de caracteres  | Por exemplo, `Email`, `OfficeCommunicationsOnline`.                                  |
| isDefault    | Booliano | `true` se esse for o domínio padrão associado ao locatário; caso contrário, `false`. |
| isInitial    | Booliano | `true` se este for o domínio inicial associado ao locatário; caso contrário, `false`. |
| nome         | Cadeia de caracteres  | O nome de domínio; por exemplo, `contoso.onmicrosoft.com`.                             |
| type         | Cadeia de caracteres  | Por exemplo, `Managed`.                                                              |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "String",
  "isDefault": true,
  "isInitial": true,
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

