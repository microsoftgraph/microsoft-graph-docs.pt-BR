---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a42203020f06e5892d0ba1927631520dbb59c87b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982253"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = graphClient.groups("0d75b8dc-c42d-44dd-890a-751a99c0589f").threads("AAQkAD8EJUmcWwTJi06Cew==").posts("AQMkADgAAAIJbQAAAA==")
    .buildRequest()
    .get();

```