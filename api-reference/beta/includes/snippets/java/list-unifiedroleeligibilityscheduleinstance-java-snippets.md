---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eda595e90d088f3d9a3cccebf99ade6b5be93f989857f78a940194381c45281f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327934"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleInstanceCollectionPage roleEligibilityScheduleInstances = graphClient.roleManagement().directory().roleEligibilityScheduleInstances()
    .buildRequest()
    .get();

```