---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9aecca5fd87537c9bf256f1de5116efcf6f4d9f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972208"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublicationCollectionPage publications = graphClient.me().profile().publications()
    .buildRequest()
    .get();

```