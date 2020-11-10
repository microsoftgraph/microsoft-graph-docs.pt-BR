---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58c35ab00f438a40f2b2a15637ebc3248ba573a0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957398"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IApplicationCollectionWithReferencesPage applications = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}").applications()
    .buildRequest()
    .get();

```