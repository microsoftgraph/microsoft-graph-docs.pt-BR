---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40398c14fda34e4c5c4395c5db8c4608742f3fd17f94006389b921f8b27dde3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376756"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Application application = new Application();
application.displayName = "New display name";

graphClient.applications("{id}")
    .buildRequest()
    .patch(application);

```