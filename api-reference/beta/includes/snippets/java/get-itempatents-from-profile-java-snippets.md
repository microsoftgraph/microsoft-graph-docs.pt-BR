---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9857a55fa9406b391990356395c6edd57831f44d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980542"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPatentCollectionPage patents = graphClient.me().profile().patents()
    .buildRequest()
    .get();

```