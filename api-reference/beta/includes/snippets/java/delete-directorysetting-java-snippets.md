---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac10ce97bd19be9fc50863539bff538d701e2523
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410766"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.settings("3c105fc3-2254-4861-9e2d-d59e2126f3ef")
    .buildRequest()
    .delete();

```