---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16b7a4188e45d716f82078ca0b5fa02e97fdbf32263af52f30014f3caf139e54
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214498"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<SynchronizationSecretKeyStringValuePair> credentialsList = new LinkedList<SynchronizationSecretKeyStringValuePair>();
SynchronizationSecretKeyStringValuePair credentials = new SynchronizationSecretKeyStringValuePair();

credentialsList.add(credentials);

graphClient.applications("{applicationsId}").synchronization()
    .acquireAccessToken(SynchronizationAcquireAccessTokenParameterSet
        .newBuilder()
        .withCredentials(credentialsList)
        .build())
    .buildRequest()
    .post();

```