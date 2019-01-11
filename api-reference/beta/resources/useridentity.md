---
title: tipo de userIdentity
description: 'Para o Windows Azure AD avaliações de acesso, esse tipo representa uma identidade de usuário do Windows Azure AD por um revisor de uma revisão de acesso.  '
localization_priority: Normal
ms.openlocfilehash: 5b629fff4c5cecd513777cc5004646aac5f1c85b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839638"
---
# <a name="useridentity-type"></a>tipo de userIdentity

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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

<!-- {
  "type": "#page.annotation",
  "description": "userIdentity type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
