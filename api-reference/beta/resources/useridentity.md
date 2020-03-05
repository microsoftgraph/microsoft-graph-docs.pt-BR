---
title: tipo UserIdentity
description: 'Para as revisões do Azure AD Access, este tipo representa uma identidade de usuário do Azure AD para um revisor de uma revisão do Access.  '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 466b39a52f2bc2b9e20f313f3f80926855f492f9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519523"
---
# <a name="useridentity-type"></a>tipo UserIdentity

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Para as revisões do Azure AD [Access](accessreviews-root.md), este tipo representa uma identidade de usuário do Azure ad para um criador ou revisor de uma revisão do Access.  
No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que foram iniciadas ou foram afetadas por uma atividade de auditoria.

Esse tipo herda de [Identity](identity.md) e tem uma propriedade adicional, o nome principal do usuário do usuário.

## <a name="methods"></a>Métodos

Nenhum.  Você deve incluir objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `displayName` | `String` | Nome de exibição da identidade. Observe que isso pode não estar sempre disponível ou atualizado.    |
| `id`          | `String` | Identificador exclusivo da identidade.  |
| `ipAddress`| `String`| Indica o endereço IP do cliente usado pelo usuário que está executando a atividade (log de auditoria somente).|
| `userPrincipalName`|`String` | O atributo userPrincipalName do usuário. |

## <a name="remarks"></a>Comentários

Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.

## <a name="relationships"></a>Relações

Nenhum

## <a name="see-also"></a>Ver também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter revisores do accessReview](../api/accessreview-listreviewers.md) |       coleção [UserIdentity](useridentity.md)| Obter os revisores de um accessReview. |
|[Adicionar revisor accessReview](../api/accessreview-addreviewer.md) |      Nenhum.   |   Adicionar um revisor a um accessReview. |
|[Remover revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum.  |   Remover um revisor de um accessReview. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do tipo.

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
  "userPrincipalName": "String",
  "ipAddress": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
