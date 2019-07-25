---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5179307e0b6b835178cfae98ca25d1251c42fec9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867087"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage registeredDevices = graphClient.me().registeredDevices()
    .buildRequest()
    .get();

```