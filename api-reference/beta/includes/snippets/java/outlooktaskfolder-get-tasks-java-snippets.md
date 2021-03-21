---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0e1a4698f3f88273bf493eca5205c390eae73ef1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966640"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskCollectionPage tasks = graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPWAAA=").tasks()
    .buildRequest()
    .get();

```