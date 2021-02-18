---
title: Tipo de recurso userIdentity
description: No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que iniciaram ou foram afetadas por uma atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 814b7106bf738711099d6d6e8d5e821b7b638318
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292158"
---
# <a name="useridentity-resource-type"></a>Tipo de recurso userIdentity

Namespace: microsoft.graph

No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que iniciaram ou foram afetadas por uma atividade de auditoria.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| displayName | String | Nome de exibição da identidade. Observe que isso pode nem sempre estar disponível ou atualizado.    |
| id          | String | Identificador exclusivo da identidade.  |
| ipAddress   | Cadeia de caracteres| Indica o endereço IP do cliente usado pelo usuário executando a atividade (somente log de auditoria).|
| userPrincipalName | String  | O atributo userPrincipalName do usuário. |

>**Observação:** Em alguns casos, o identificador exclusivo pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON do tipo.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
"displayName", "thumbnails"
  ],
  "@odata.type": "microsoft.graph.userIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string",
  "ipAddress": "string",
  "userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

