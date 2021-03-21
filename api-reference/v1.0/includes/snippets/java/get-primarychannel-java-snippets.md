---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ca697504270f489fe943329e1bd1198e7368acf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984319"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = graphClient.teams("{id}").primaryChannel()
    .buildRequest()
    .get();

```