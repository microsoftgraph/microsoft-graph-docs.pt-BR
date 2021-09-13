---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9815bf1c8ccc0fdf66e3c2dc31b833517d7bd8785881a869579f31de6307678
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217075"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .resetUnseenCount()
    .buildRequest()
    .post();

```