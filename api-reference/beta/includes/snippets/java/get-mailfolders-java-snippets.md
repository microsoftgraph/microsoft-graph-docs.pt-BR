---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a94a3afcf2b9c6ed27e53d225a2718854e59b4fc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982173"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailFolderCollectionPage mailFolders = graphClient.me().mailFolders()
    .buildRequest()
    .get();

```