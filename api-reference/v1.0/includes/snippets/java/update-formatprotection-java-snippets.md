---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4e41bcd0118786ba6159f2349bbde28dd034eda
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982533"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookFormatProtection workbookFormatProtection = new WorkbookFormatProtection();
workbookFormatProtection.locked = true;
workbookFormatProtection.formulaHidden = true;

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().protection()
    .buildRequest()
    .patch(workbookFormatProtection);

```