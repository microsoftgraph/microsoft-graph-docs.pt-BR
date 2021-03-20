---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c30492c037621997e162af013b1787508983a8d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
    .delta()
    .buildRequest()
    .get();

```