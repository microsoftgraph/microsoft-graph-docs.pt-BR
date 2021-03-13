---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f82cf2895dd9abd12528ff231700ed298ebfc762
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772952"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserSource userSource = new UserSource();
userSource.email = "megan@contoso.com";
userSource.includedSources = EnumSet.of(SourceType.MAILBOX,SourceType.SITE);

graphClient.compliance().ediscovery().cases("4c8f8f70-7785-4bd4-b296-c98376a2c5e1").custodians("2192ca408ea2410eba3bec8ae873be6b").userSources()
    .buildRequest()
    .post(userSource);

```