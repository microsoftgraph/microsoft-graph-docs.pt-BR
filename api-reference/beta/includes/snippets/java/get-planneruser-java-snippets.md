---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61deaae0a8e0cb45996f7fce592b57b0b2016628
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982667"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerUser plannerUser = graphClient.me().planner()
    .buildRequest()
    .get();

```