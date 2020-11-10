---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 450222da34c13991aec1133e12ebaf74344e5e6f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970110"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserFindRoomListsCollectionPage findRoomLists = graphClient.me()
    .findRoomLists()
    .buildRequest()
    .get();

```