---
title: tipo de recurso authenticationSourceFilter
description: Filtro com base na origem da autenticação que é usada para determinar se o ouvinte foi executado ou não.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0fcbeb3296b6b0dece1b69cedf26d600c240d43d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720091"
---
# <a name="authenticationsourcefilter-resource-type"></a>tipo de recurso authenticationSourceFilter

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Filtro com base na origem da autenticação que é usada para determinar se o ouvinte é avaliado.

A propriedade **includeApplications** pode ser usada para habilitar a inscrição de autoatendimento em um aplicativo no Azure Active Directory. Saiba mais lendo nossa documentação para [habilitar aplicativos em um fluxo de usuário de inscrição de autoatendimento](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow).

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|includeApplications|Coleção de cadeias de caracteres|Aplicativos a serem incluídos para avaliação do [authenticationListener](../resources/authenticationlistener.md). Esses aplicativos acionam a ação associada quando usados como o aplicativo cliente no fluxo de autenticação. O identificador de aplicativo é a ID do cliente do aplicativo.|

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
