---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afb26494911d628564a8a214d2273eec0078adc9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967609"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPositionCollectionPage positions = graphClient.me().profile().positions()
    .buildRequest()
    .get();

```