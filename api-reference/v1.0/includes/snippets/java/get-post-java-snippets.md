---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 266101edbd08dcfaa40e1dbe861cb746b0c96211
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981885"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = graphClient.groups("{id}").threads("{id}").posts("{id}")
    .buildRequest()
    .get();

```