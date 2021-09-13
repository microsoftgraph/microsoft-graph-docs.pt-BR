---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b676358f7addeecd3f7d7cfa1377bb122a1581501394b8b8d3685cfdc5f0cf45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216628"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().onenote().pages("{id}")
    .buildRequest()
    .delete();

```