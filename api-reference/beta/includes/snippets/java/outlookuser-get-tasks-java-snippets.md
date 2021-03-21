---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcca844d34e3d733e95c663d9878bc82735cb823
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982365"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskCollectionPage tasks = graphClient.me().outlook().tasks()
    .buildRequest()
    .get();

```