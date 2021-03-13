---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82ac9a9b7ddaff43ad6816437a6e0759c5e62a7d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771551"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionWithReferencesPage allowedUsers = graphClient.print().shares("{printerShareId}").allowedUsers()
    .buildRequest()
    .get();

```