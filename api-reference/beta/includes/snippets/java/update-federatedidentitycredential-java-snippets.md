---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 004650852013942d7a7f9883bb79132a35bfb7d6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694763"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FederatedIdentityCredential federatedIdentityCredential = new FederatedIdentityCredential();
federatedIdentityCredential.name = "testing02";
federatedIdentityCredential.issuer = "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0";
federatedIdentityCredential.subject = "a7d388c3-5e3f-4959-ac7d-786b3383006a";
federatedIdentityCredential.description = "Updated description";
LinkedList<String> audiencesList = new LinkedList<String>();
audiencesList.add("api://AzureADTokenExchange");
federatedIdentityCredential.audiences = audiencesList;

graphClient.applications("bcd7c908-1c4d-4d48-93ee-ff38349a75c8").federatedIdentityCredentials("15be77d1-1940-43fe-8aae-94a78e078da0")
    .buildRequest()
    .patch(federatedIdentityCredential);

```