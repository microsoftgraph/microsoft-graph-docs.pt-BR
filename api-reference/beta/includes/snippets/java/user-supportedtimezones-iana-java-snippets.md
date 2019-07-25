---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38f1ec294d3e0663b15bf019575bdafd2fb80d79
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877255"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITimeZoneInformationCollectionPage supportedTimeZones = graphClient.me().outlook()
    .supportedTimeZones(microsoft.graph.timeZoneStandard'Iana')
    .buildRequest()
    .get();

```