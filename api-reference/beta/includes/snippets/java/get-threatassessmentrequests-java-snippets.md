---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e97940aaf45d461b364ee40586a72f0afb3c1224ac89432dd48e3d4a0f22a490
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214162"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequestCollectionPage threatAssessmentRequests = graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .get();

```