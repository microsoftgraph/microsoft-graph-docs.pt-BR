---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6cda50e7ae7efe4a0033758e2d8018bd1a34e71392ec0d77361e53bb5de4e14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407626"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffRequest timeOffRequest = graphClient.teams("{teamId}").schedule().timeOffRequests("{timeOffRequestId}")
    .buildRequest()
    .get();

```