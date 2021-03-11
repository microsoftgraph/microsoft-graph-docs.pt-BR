---
title: Tipo userIdentity
description: Representa uma identidade de usuário do Azure AD para um revistor de uma revisão de acesso.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 9379955a4356ff9c969e4813fbf9b812316aa821
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719854"
---
# <a name="useridentity-type"></a>Tipo userIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Para as análises de acesso do Azure AD, esse tipo representa uma identidade de usuário do Azure AD para um criador ou [revistor](accessreviews-root.md)de uma revisão de acesso.
No contexto de um log de auditoria do Azure AD, isso representa as informações do usuário que iniciaram ou foram afetadas por uma atividade de auditoria.

Esse tipo herda da [identidade](identity.md) e tem uma propriedade adicional, o nome principal do usuário.

## <a name="methods"></a>Métodos

Nenhum.  Você incluiria objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição|
|:---------------|:--------|:----------|
| `displayName` | `String` | Nome de exibição da identidade. Observe que isso pode nem sempre estar disponível ou atualizado.    |
| `id`          | `String` | Identificador exclusivo da identidade.  |
| `ipAddress`| `String`| Indica o endereço IP do cliente usado pelo usuário executando a atividade (somente log de auditoria).|
| `userPrincipalName`|`String` | O atributo userPrincipalName do usuário. |

## <a name="remarks"></a>Comentários

Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.

## <a name="relationships"></a>Relações

Nenhum

## <a name="see-also"></a>Ver também

| Método                                                                | Tipo de retorno                                | Descrição                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [Obter revisores do accessReview](../api/accessreview-listreviewers.md)    | [Coleção userIdentity](useridentity.md) | Obter os revisores de um accessReview.   |
| [Adicionar o revisor accessReview](../api/accessreview-addreviewer.md)       | Nenhum.                                      | Adicione um revisor a um accessReview.      |
| [Remover o revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum.                                      | Remova um revisor de um accessReview. |

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


