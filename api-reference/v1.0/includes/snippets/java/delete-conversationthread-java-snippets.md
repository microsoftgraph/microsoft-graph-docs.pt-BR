---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c739ffc1ae9fff34f106442dd767873d66e2be9d96768eee76451f0677d7f6a2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327912"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").threads("{id}")
    .buildRequest()
    .delete();

```