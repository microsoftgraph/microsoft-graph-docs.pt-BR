---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 83a91c65fbf67d3d4ef633ce0b92f1b4abdba88620e89cf5feeccc46e3c08e64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100196"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("{id}").audioRoutingGroups("{id}")
    .buildRequest()
    .delete();

```