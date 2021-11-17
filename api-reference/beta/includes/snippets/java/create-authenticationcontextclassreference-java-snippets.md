---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce3373c571feaaaa56005496627ed9b858d7d6de2f44d01c5773805304a856a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375826"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationContextClassReference authenticationContextClassReference = new AuthenticationContextClassReference();
authenticationContextClassReference.id = "c1";
authenticationContextClassReference.displayName = "Contoso medium";
authenticationContextClassReference.description = "Medium protection level defined for Contoso policy";
authenticationContextClassReference.isAvailable = true;

graphClient.identity().conditionalAccess().authenticationContextClassReferences()
    .buildRequest()
    .post(authenticationContextClassReference);

```