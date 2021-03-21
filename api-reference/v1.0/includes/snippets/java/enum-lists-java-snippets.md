---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 313a7632810dd435a974b345ca62e1a31faa10f3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982395"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ListCollectionPage lists = graphClient.sites("{site-id}").lists()
    .buildRequest()
    .get();

```