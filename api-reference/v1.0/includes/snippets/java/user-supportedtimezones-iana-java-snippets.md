---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8471872975a3425d1c9f542642e5abbbb1a01a56
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983871"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookUserSupportedTimeZonesCollectionPage supportedTimeZones = graphClient.me().outlook()
    .supportedTimeZones(OutlookUserSupportedTimeZonesParameterSet
        .newBuilder()
        .withTimeZoneStandard(microsoft.graph.timeZoneStandard'Iana')
        .build())
    .buildRequest()
    .get();

```