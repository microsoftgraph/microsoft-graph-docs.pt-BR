---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c67678f445714438a8925efc45080c32d5ec37d0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983781"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionPage users = graphClient.users()
    .buildRequest()
    .filter("startswith(displayName,'Eric'),")
    .select("displayName,signInActivity")
    .get();

```