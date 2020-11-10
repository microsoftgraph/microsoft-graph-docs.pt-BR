---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37fc073d0d4bd6730fcacb8391c491da0c69ccf6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967340"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonWebsiteCollectionPage websites = graphClient.me().profile().websites()
    .buildRequest()
    .get();

```