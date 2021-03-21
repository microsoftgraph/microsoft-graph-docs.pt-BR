---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbcac2e09cf0ed002a2158a9d81c8372a0ef0773
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979628"
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