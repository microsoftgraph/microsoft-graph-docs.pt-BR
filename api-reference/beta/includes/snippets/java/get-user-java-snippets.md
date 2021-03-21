---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab6d4aa1d30cea153c4125ce62fd2154f2ddce34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976614"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.me()
    .buildRequest()
    .get();

```