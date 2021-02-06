---
title: Tipo de recurso authenticationSourceFilter
description: Filtrar com base na origem da autenticação que é usada para determinar se o ouvinte é executado ou não.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4736be415faab65c6ce3b572a1273a73c707ee43
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128628"
---
# <a name="authenticationsourcefilter-resource-type"></a>Tipo de recurso authenticationSourceFilter

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado.

A **propriedade includeApplications** pode ser usada para habilitar a inscrição self-service em um aplicativo no Azure Active Directory. Saiba mais lendo a nossa documentação para [habilenciar aplicativos em um fluxo de usuário de inscrição de autoatendenciamento.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|includeApplications|Coleção de cadeias de caracteres|Aplicativos a incluir para avaliação [da authenticationListener](../resources/authenticationlistener.md). Esses aplicativos acionam a ação associada quando usada como o aplicativo cliente no fluxo de autenticação. O identificador do aplicativo é a ID do cliente do aplicativo.|

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
