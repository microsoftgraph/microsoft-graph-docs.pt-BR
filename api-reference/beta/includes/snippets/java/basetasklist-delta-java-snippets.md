---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0254056b6d608fe3fbde5a3a36ffb833d07d0ebb
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525245"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content delta = graphClient.me().tasks().lists().delta()
    .buildRequest()
    .get();

```