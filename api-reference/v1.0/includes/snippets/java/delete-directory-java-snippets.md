---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b121391e19dd7d9db429ec9b6501977a8b8259a924f37f06223aaff513f5ebbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158136"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .delete();

```