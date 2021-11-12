---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1caca3e0e1bdf6fdd80018b710476eea203c5c37080d6bffd8fec9756a150408
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157542"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .buildRequest()
    .expand("tasks")
    .get();

```