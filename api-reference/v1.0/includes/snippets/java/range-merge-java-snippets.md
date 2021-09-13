---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6bd883ceaed913de94dc6c1603fa83a9860b71c56bc4c071c029dbee31810648
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897751"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean across = true;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .merge(WorkbookRangeMergeParameterSet
        .newBuilder()
        .withAcross(across)
        .build())
    .buildRequest()
    .post();

```