---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86e02d21654dde922cc537b6fb0d8570f7146c36
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968131"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintTaskCollectionPage tasks = graphClient.print().taskDefinitions("92d72a3d-cad7-4809-8924-43833282b079").tasks()
    .buildRequest()
    .get();

```