---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3660dd21820c579ffbce32d18bb86c45d906b8b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CredentialUserRegistrationDetailsCollectionPage credentialUserRegistrationDetails = graphClient.reports().credentialUserRegistrationDetails()
    .buildRequest()
    .get();

```