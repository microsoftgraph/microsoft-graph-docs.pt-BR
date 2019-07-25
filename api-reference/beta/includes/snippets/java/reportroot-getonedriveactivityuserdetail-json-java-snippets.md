---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef67f3ec45e5d615f88a985909366201da715454
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873059"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveActivityUserDetailCollectionPage getOneDriveActivityUserDetail = graphClient.reports()
    .getOneDriveActivityUserDetail('D7')
    .buildRequest()
    .get();

```