---
title: Tipo de recurso printUserIdentity
description: Representa uma identidade de usuário dentro do serviço de Impressão Universal. Mapas a um Azure AD usuário.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 50a73a6f08448d50ac616e82d15c046d52d63b83
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176309"
---
# <a name="printuseridentity-resource-type"></a>Tipo de recurso printUserIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma identidade de usuário dentro do serviço de Impressão Universal. Mapas a [um usuário Azure Active Directory (Azure AD).](user.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres|O identificador printUserIdentity. Somente leitura.|
|displayName|Cadeia de caracteres|O nome de exibição de printUserIdentity.|
|ipAddress|Cadeia de caracteres|O endereço IP printUserIdentity. Não populado.|
|userPrincipalName|Cadeia de caracteres|O NOME UPN (nome UPN) do usuário printUserIdentity.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUserIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUserIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


