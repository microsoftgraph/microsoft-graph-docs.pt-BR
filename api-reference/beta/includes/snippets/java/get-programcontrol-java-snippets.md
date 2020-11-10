---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 832e278b20a2ee7f7afb0ff73337a4fde340af1e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981728"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProgramControlCollectionPage programControls = graphClient.programControls()
    .buildRequest()
    .get();

```