---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29378e0b458faaee53c06724c45b8854b8cc3052
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978331"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().userFlowAttributes("{id}")
    .buildRequest()
    .delete();

```