---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a4b6432548321cc74e425849d7de5e74e297a6b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982065"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UsedInsightCollectionPage used = graphClient.me().insights().used()
    .buildRequest()
    .orderBy("LastUsed/LastAccessedDateTime desc")
    .get();

```