---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa763aeb1456caf903aa3c738fa8c616a8dfeac4385202da605c2f5ca698463f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407750"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call call = graphClient.communications().calls("{id}")
    .buildRequest()
    .get();

```