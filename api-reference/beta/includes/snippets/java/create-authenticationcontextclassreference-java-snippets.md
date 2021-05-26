---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e0c9a42bca35c09a6cab92041a5f44ad45a965e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663934"
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