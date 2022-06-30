---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3259fb187a1190786300df4bf887b6ac4895338c
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694812"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DeviceRegistrationPolicy deviceRegistrationPolicy = graphClient.policies().deviceRegistrationPolicy()
    .buildRequest()
    .get();

```