---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11552d19c03bfb30812e88ef0b9dfe4018122902
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975756"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}")
    .buildRequest()
    .delete();

```