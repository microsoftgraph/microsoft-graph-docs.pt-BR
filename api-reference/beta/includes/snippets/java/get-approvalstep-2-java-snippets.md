---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb475e916cff7f748ed2a216587aacd5830596e1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942531"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ApprovalStep approvalStep = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489").steps("d4fa4045-4716-436d-aec5-57b0a713f095")
    .buildRequest()
    .get();

```