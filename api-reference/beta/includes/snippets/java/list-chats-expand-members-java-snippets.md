---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39a9dbf54f24dfe38c21a42f706afd4eeb133693
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752882"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IChatCollectionPage chats = graphClient.users("8b081ef6-4792-4def-b2c9-c363a1bf41d5").chats()
    .buildRequest()
    .expand("members")
    .get();

```