---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f9a9aa69fee43ea20159b43cb9a6f224b5d6060
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868052"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOff timeOff = graphClient.teams("{teamId}").schedule().timesOff("{timeOffId}")
    .buildRequest()
    .get();

```