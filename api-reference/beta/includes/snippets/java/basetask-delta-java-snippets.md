---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44bdedfba87e589d0db95e23c14c8b67e9ee9452
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525342"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content delta = graphClient.me().tasks().lists().aAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQpLAt-6oC2JgAQCQ47jE5P--SoVECqTdM17RAAAB4mDIAAA=().tasks().delta()
    .buildRequest()
    .get();

```