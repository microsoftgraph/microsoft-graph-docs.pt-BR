---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 512e6cb5ea04852f0ea3128b748b4c53ab9f4dd5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980773"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPersonInterestCollectionPage interests = graphClient.me().profile().interests()
    .buildRequest()
    .get();

```