---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48455efcddf9a9cc24452b03c17165a20f18b03a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962280"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintServiceCollectionPage services = graphClient.print().services()
    .buildRequest()
    .get();

```