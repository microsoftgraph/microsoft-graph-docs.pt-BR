---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea6ee560296dd4efccbdc5c60499d784b1561e64
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877253"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITimeZoneInformationCollectionPage supportedTimeZones = graphClient.me().outlook()
    .supportedTimeZones()
    .buildRequest()
    .get();

```