---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95802d1a5639345402347c7dce8dec0bf68a0b7d96e8dda638f01746f1187d02
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157076"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocation namedLocation = graphClient.identity().conditionalAccess().namedLocations("0854951d-5fc0-4eb1-b392-9b2c9d7949c2")
    .buildRequest()
    .get();

```