---
title: Tipo de recurso conditionalAccess
description: O **recurso conditionalaccess** é o ponto de entrada para o modelo de objeto Conditinal Access. Ele não contém propriedades usáveis.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3683965cda79f003cb5e548101272d869be902b8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547350"
---
# <a name="conditionalaccess-resource-type"></a>Tipo de recurso conditionalaccess

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso conditionalAccess** é o ponto de entrada do modelo de objeto Conditional Access. Ele não contém propriedades usáveis.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar conditionalAccessPolicy](../api/conditionalaccessroot-post-policies.md) |[conditionalAccessPolicy](conditionalaccesspolicy.md)| Crie um novo **conditionalAccessPolicy** postando na coleção conditionalAccessPolicy.|
|[Criar namedLocations](../api/conditionalaccessroot-post-namedlocations.md) |[namedLocation](namedlocation.md)| Crie um novo **namedLocations** postando na coleção namedLocations.|
|[Criar authenticationContextClassReferences](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md)|[authenticationContextClassReferences](authenticationcontextclassreference.md)|Crie uma nova **autenticaçãoContextClassReferences** postando na coleção authenticationContextClassReferences.|


## <a name="properties"></a>Propriedades

O recurso conditionalAccess é o ponto de entrada para o modelo de objeto do Access Condicional e não contém nenhuma propriedade.

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|conditionalAccessPolicy|[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto| Somente leitura. Anulável. Retorna uma coleção das políticas de Acesso Condicional especificadas.|
|namedLocations|[Coleção namedLocations](namedlocation.md)| Somente leitura. Anulável. Retorna uma coleção dos locais nomeados especificados.|
|authenticationContextClassReferences|[Coleção authenticationContextClassReferences](authenticationcontextclassreference.md)|Somente leitura. Anulável. Retorna uma coleção das referências de classe de contexto de autenticação especificadas.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conditional access resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

