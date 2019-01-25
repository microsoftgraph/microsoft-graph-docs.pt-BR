---
title: tipo de userIdentity
description: 'Para o Windows Azure AD avaliações de acesso, esse tipo representa uma identidade de usuário do Windows Azure AD por um revisor de uma revisão de acesso.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab8076c5ff24e20006b5a5569dacf4c45d987512
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529464"
---
# <a name="useridentity-type"></a>tipo de userIdentity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Para o Windows Azure AD [access analisa](accessreviews-root.md), esse tipo representa uma identidade de usuário do Windows Azure AD para um revisor de uma revisão de acesso.  
No contexto de um log de auditoria do Azure AD, isso representa as informações de usuário que iniciou ou foi afetadas por uma atividade de auditoria.

Esse tipo de herda de [identidade](identity.md) e tem uma propriedade adicional, o nome de usuário principal do usuário.

## <a name="methods"></a>Métodos

Nenhum.  Você incluiria objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `displayName` | `String` | Nome para exibição da identidade. Observe que isso nem sempre pode ser disponível ou atualizadas.    |
| `id`          | `String` | Identificador exclusivo da identidade.  |
| `ipAddress`| `String`| Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (somente no log de auditoria).|
| `userPrincipalName`|`String` | O atributo userPrincipalName do usuário. |

## <a name="remarks"></a>Comentários

Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.

## <a name="relationships"></a>Relações

Nenhum.

## <a name="see-also"></a>Ver também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview reviewers](../api/accessreview-listreviewers.md) |       coleção [userIdentity](useridentity.md)| Obtenha os revisores de um accessReview. |
|[Adicionar Revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicione um revisor a um accessReview. |
|[Remover accessReview revisor](../api/accessreview-removereviewer.md) | Nenhum.  |   Remova um revisor de um accessReview. |

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
 "userPrincipalName": "String"
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
