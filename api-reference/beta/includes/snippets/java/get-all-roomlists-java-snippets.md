---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 146e41ede75ad869edc8807180c1b5c6dde5b1a99fe10f9d6ce75a92a0fc84de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216328"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RoomListCollectionPage roomlist = graphClient.places().microsoft.graph.roomlist()
    .buildRequest()
    .get();

```