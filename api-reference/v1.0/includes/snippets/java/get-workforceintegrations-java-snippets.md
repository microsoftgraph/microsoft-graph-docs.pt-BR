---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d88ceb12a5c83de6a177fdbfca63896ef218851
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217556"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkforceIntegrationCollectionPage workforceIntegrations = graphClient.teamwork().workforceIntegrations()
    .buildRequest()
    .get();

```