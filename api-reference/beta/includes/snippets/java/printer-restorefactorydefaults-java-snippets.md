---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79b156377798b08c1b7dc4d189fa2a64801a19f50d66145c32df08597dd32984
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897906"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}")
    .restoreFactoryDefaults()
    .buildRequest()
    .post();

```