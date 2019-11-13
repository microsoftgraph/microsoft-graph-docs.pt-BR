---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 213479637477d1a48f3c1c74aace7746336cd63f
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302272"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String calculationType = "calculationType-value";

graphClient.me().drive().items("{id}").workbook().application()
    .calculate(calculationType)
    .buildRequest()
    .post();

```