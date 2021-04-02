---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d46958244676f79d2a9dca7fd1d639e84ed55d16
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507453"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5")
    .completeMigration()
    .buildRequest()
    .post();

```