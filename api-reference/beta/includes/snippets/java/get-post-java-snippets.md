---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3f48a3515e72c7cd08cf01a5321835f9f32232d7a21e0e08666b08dbd5948fb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160169"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = graphClient.groups("0d75b8dc-c42d-44dd-890a-751a99c0589f").threads("AAQkAD8EJUmcWwTJi06Cew==").posts("AQMkADgAAAIJbQAAAA==")
    .buildRequest()
    .get();

```