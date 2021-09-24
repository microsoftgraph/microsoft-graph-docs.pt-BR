---
title: Tipo de recurso authenticationSourceFilter
description: Filtrar com base na origem da autenticação usada para determinar se o ouvinte é executado ou não.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 53f765f998dffdce5dcfd549177ebd1250cf013f
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508009"
---
# <a name="authenticationsourcefilter-resource-type"></a>Tipo de recurso authenticationSourceFilter

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado.

A **propriedade includeApplications** pode ser usada para habilitar a inscrição em um aplicativo em Azure Active Directory. Saiba mais lendo nossa documentação para habilenciar aplicativos em um fluxo de usuário de [autoatendenciamento.](/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|includeApplications|Coleção de cadeias de caracteres|Aplicativos a incluir para avaliação do [authenticationListener](../resources/authenticationlistener.md). Esses aplicativos acionam a ação associada quando usada como o aplicativo cliente no fluxo de autenticação. O identifer do aplicativo é a ID do cliente do aplicativo.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationSourceFilter"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationSourceFilter",
  "includeApplications": [
    "String"
  ]
}
```
