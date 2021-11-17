---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 411787ec3c71394e4cb3a9edc6a52ca3f211b83d2447fc6d0f08b09581848e78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100343"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{teamId}").schedule().timesOff("{timeOffId}")
    .buildRequest()
    .delete();

```