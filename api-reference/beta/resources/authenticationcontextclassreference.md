---
title: Tipo de recurso authenticationContextClassReference
description: Representa uma Azure Active Directory de classe de contexto de autenticação.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1397545d7b102d05b8c71957cea88f9c131f0e09
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547351"
---
# <a name="authenticationcontextclassreference-resource-type"></a>Tipo de recurso authenticationContextClassReference

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma Azure Active Directory de classe de contexto de autenticação. Referências de classe de contexto de autenticação são valores personalizados que definem um requisito de autenticação de Acesso Condicional.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar authenticationContextClassReference](../api/conditionalaccessroot-list-authenticationcontextclassreferences.md) | [Coleção authenticationContextClassReference](authenticationContextClassReference.md) | Obter todos os objetos authenticationContextClassReference na organização. |
| [Criar authenticationContextClassReference](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | Crie um novo objeto authenticationContextClassReference. |
| [Obter authenticationContextClassReference](../api/authenticationcontextclassreference-get.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | Ler propriedades e relações de um objeto authenticationContextClassReference. |
| [Atualizar authenticationContextClassReference](../api/authenticationcontextclassreference-update.md) | [authenticationContextClassReference](authenticationContextClassReference.md) | Atualize um objeto authenticationContextClassReference. |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Identificador usado para fazer referência à classe de contexto de autenticação. A id é usada para disparar a autenticação de etapa para os requisitos de autenticação referenciados e é o valor que será emitido na declaração do acrs. Esse valor na declaração é usado para verificar se o contexto de autenticação necessário foi satisfeito. Os valores de id permitidos são "c1" até "c25". |
|displayName|String| O nome para exibição é o nome amigável da authenticationContextClassReference. Esse valor deve ser usado para identificar a referência de classe de contexto de autenticação ao criar experiências de administrador voltadas para o usuário. Por exemplo, UX de seleção. |
|descrição|String| Uma breve explicação das políticas impostas pela authenticationContextClassReference. Esse valor deve ser usado para fornecer texto secundário para descrever a referência de classe de contexto de autenticação ao criar experiências de administrador voltadas para o usuário. Por exemplo, UX de seleção.|
|isAvailable|booliano| Indica se a authenticationContextClassReference foi publicada pelo administrador de segurança e está pronta para uso pelos aplicativos. Quando estiver definido para ele, não deverá ser mostrado nas experiências de UX do administrador, pois o valor não está disponível no momento `false` para seleção.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
    {
      "id": "String",
      "displayName": "String",
      "description": "String",
      "isAvailable": "boolean",
    }

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationContextClassReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
