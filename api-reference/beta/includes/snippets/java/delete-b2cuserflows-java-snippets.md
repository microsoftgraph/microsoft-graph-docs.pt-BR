---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: baff3a04ee2e28d9564f70a47d3934e10d3a8884
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975117"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("{id}")
    .buildRequest()
    .delete();

```