---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9780768eb61f0b11960a08dde2571d862b1736c5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969532"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = graphClient.applications("{id}")
    .buildRequest()
    .get();

```