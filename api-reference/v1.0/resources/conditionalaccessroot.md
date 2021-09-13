---
title: Tipo de recurso conditionalAccessRoot
description: O recurso conditionalAccessRoot é o ponto de entrada para o modelo de objeto acesso condicional (CA). Ele não contém propriedades usáveis.
ms.localizationpriority: medium
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 739b02a5bf06c7ac742b524e406145c29bb40aa3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59110496"
---
# <a name="conditionalaccessroot-resource-type"></a>Tipo de recurso conditionalAccessRoot

Namespace: microsoft.graph

O **recurso conditionalAccessRoot** é o ponto de entrada para o modelo de objeto acesso condicional (CA). Ele não contém propriedades usáveis.

Para obter mais informações sobre o Acesso Condicional no Azure Active Directory, consulte [O que é Acesso Condicional](/azure/active-directory/conditional-access/overview)?

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|namedLocations|[coleção namedLocation](namedlocation.md)| Somente leitura. Anulável. Retorna uma coleção dos locais nomeados especificados.|
|policies|[conditionalAccessPolicy](conditionalaccesspolicy.md) conjunto| Somente leitura. Anulável. Retorna uma coleção das políticas de Acesso Condicional (CA) especificadas.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.conditionalAccessRoot"
}-->

```json
{
  "@odata.type": "#microsoft.graph.conditionalAccessRoot"
}
```