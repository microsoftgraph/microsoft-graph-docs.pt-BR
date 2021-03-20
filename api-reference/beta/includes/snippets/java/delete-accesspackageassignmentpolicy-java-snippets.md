---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25f9682388b8e5f2608156f7717d2bc8b2038668
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977797"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies("{id}")
    .buildRequest()
    .delete();

```