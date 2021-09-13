---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 630728c45205762340d54e5c03b603bf252204ef42609fd310b915a98753558b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157908"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffCollectionPage timesOff = graphClient.teams("{teamId}").schedule().timesOff()
    .buildRequest()
    .filter("sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z")
    .get();

```