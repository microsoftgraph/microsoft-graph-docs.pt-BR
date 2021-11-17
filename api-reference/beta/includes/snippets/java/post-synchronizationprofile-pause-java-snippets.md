---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94c129f6052be5214fb9eaa5321443d03a3ac14c92e1437185cf03c41b32ccb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102883"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .pause()
    .buildRequest()
    .post();

```