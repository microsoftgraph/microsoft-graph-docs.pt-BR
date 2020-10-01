---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be15adb230205cca96664080e93438ef28ceff02
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315514"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamsId}").members("{membership-id}")
    .buildRequest()
    .delete();

```