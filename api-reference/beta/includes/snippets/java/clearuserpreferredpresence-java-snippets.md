---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f71f65a91f167e498933672d6c99ef01a124ccdb
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524832"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("fa8bf3dc-eca7-46b7-bad1-db199b62afc3").presence()
    .clearUserPreferredPresence()
    .buildRequest()
    .post();

```