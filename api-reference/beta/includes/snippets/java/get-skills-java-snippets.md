---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51ae48ddfcbadd080e1ff13d0de512d015f34b08
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952386"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkillProficiencyCollectionPage skills = graphClient.me().profile().skills()
    .buildRequest()
    .get();

```