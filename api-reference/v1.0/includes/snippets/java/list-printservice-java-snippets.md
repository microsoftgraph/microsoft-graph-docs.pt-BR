---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36aad8484e91aed22fc719de400d6a9d8a79bc71
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978383"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintServiceCollectionPage services = graphClient.print().services()
    .buildRequest()
    .get();

```