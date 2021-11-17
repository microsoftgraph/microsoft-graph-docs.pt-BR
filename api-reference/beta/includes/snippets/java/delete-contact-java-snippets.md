---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cae81d013a4d58c0cff2819162b87caa957854e03a9a45d4aeec8573d14d7866
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159429"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().contacts("{id}")
    .buildRequest()
    .delete();

```