---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8afa933e3866bf1825c9b4b22f3b95b758bf6dab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978795"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = graphClient.groups("0d75b8dc-c42d-44dd-890a-751a99c0589f").threads("AAQkAD8EJUmcWwTJi06Cew==").posts("AQMkADgAAAIJbQAAAA==")
    .buildRequest()
    .get();

```