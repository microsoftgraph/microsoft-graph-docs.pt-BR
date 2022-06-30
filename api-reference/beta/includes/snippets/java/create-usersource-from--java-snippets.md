---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7edd328438d8dffacbe3254a7a73125a12f7a730
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSource userSource = new UserSource();
userSource.email = "admin@M365x809305.onmicrosoft.com";
userSource.includedSources = EnumSet.of(SourceType.MAILBOX,SourceType.SITE);

graphClient.security().cases().ediscoveryCases("{ediscoveryCaseId}").legalHolds("{ediscoveryHoldPolicyId}").userSources()
    .buildRequest()
    .post(userSource);

```