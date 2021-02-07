---
title: Tipo de recurso userIdentity
description: No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que iniciaram ou foram afetadas por uma atividade de auditoria.
localization_priority: Normal
author: dhanyahk
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 1abc846321e59434053a7a33b3aa8b993a0f9edc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136959"
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
    "Error: /api-reference/beta/resources/useridentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

