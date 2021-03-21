---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56369de1f4bf40544c7ade39aa1399b19f2647cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977241"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String calculationType = "calculationType-value";

graphClient.me().drive().items("{id}").workbook().application()
    .calculate(WorkbookApplicationCalculateParameterSet
        .newBuilder()
        .withCalculationType(calculationType)
        .build())
    .buildRequest()
    .post();

```