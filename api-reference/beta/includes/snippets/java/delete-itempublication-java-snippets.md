---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60fbecb29741e5987cf8d16ab2eca40bb0ea667bfdac7a83c2b2aac30ada68cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214760"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().publications("{id}")
    .buildRequest()
    .delete();

```