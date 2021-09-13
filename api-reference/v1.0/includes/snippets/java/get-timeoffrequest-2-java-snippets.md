---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d0fc2467b54b823cfc232a51ddf44aa2c9c5494e8f210381207b1290ef47543
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376827"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffRequestCollectionPage timeOffRequests = graphClient.teams("{teamId}").schedule().timeOffRequests()
    .buildRequest()
    .get();

```