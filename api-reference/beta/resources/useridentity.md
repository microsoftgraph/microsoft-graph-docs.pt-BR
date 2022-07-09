---
title: Tipo userIdentity
description: Representa uma Azure AD de usuário para um revisador de uma revisão de acesso.
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e42f862cfbb82982ce91a0ed7339f19f9469037b
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698251"
---
# <a name="useridentity-type"></a>Tipo userIdentity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Para as Azure AD de acesso, esse tipo representa uma Azure AD de usuário para um criador ou [revisador](accessreviews-root.md) de uma revisão de acesso.
No contexto de um log Azure AD auditoria, isso representa as informações do usuário que foram iniciadas ou afetadas por uma atividade de auditoria.

Esse tipo herda da [identidade](identity.md) e tem uma propriedade adicional, o nome principal do usuário.

## <a name="methods"></a>Métodos

Nenhum.  Você incluiria objetos desse tipo no corpo de uma solicitação ao [criar um accessReview](../api/accessreview-create.md).

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                                                                            |
|:------------------|:-------|:---------------------------------------------------------------------------------------|
| displayName       | Cadeia de caracteres | Nome de exibição da identidade. Observe que isso nem sempre pode estar disponível ou atualizado. |
| id                | Cadeia de caracteres | Identificador exclusivo da identidade. Anulável.                                                   |
| ipAddress         | Cadeia de caracteres | Indica o endereço IP do cliente usado pelo usuário que executa a atividade (somente log de auditoria). |
| userPrincipalName | Cadeia de caracteres | O atributo userPrincipalName do usuário.                                           |

### <a name="remarks"></a>Comentários

Em algumas circunstâncias, o identificador exclusivo para o ator pode não estar disponível. Nesse caso, a propriedade **displayName** para a identidade será retornada, mas a propriedade **id** estará ausente do recurso.

## <a name="relationships"></a>Relações

Nenhum

## <a name="see-also"></a>Ver também

| Método                                                                | Tipo de retorno                                | Descrição                             |
|:----------------------------------------------------------------------|:-------------------------------------------|:----------------------------------------|
| [Obter revisores accessReview](../api/accessreview-listreviewers.md)    | [coleção userIdentity](useridentity.md) | Obtenha os revisores de um accessReview.   |
| [Adicionar revisor accessReview](../api/accessreview-addreviewer.md)       | Nenhum.                                      | Adicione um revisor a um accessReview.      |
| [Remover o revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum.                                      | Remover um revisor de um accessReview. |

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


