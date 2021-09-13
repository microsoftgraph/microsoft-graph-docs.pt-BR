---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1c21b5c5cc284de4518a49ec25ae9367f830584821c67682fda8ac59bd3a1f66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407031"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String applyTo = "applyTo-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .clear(WorkbookRangeClearParameterSet
        .newBuilder()
        .withApplyTo(applyTo)
        .build())
    .buildRequest()
    .post();

```