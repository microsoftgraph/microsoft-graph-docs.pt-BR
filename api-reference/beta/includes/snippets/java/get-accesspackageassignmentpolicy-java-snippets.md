---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f879aedc17d4f0caa8977202ee37e3f905b251d3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982083"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies("{id}")
    .buildRequest()
    .get();

```