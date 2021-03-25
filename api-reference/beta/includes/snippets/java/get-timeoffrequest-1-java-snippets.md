---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ea60a53d23bfb3deef110b70a6bd9e937b75405
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211160"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffRequest timeOffRequest = graphClient.teams("{teamId}").schedule().timeOffRequests("{timeOffRequestId}")
    .buildRequest()
    .get();

```