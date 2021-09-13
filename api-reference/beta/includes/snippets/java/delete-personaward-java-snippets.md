---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20cb8b81bd0fd713b23f286b518de5fca22b6b9c4caf801e0f39374003696ebc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().awards("{personAwardId}")
    .buildRequest()
    .delete();

```