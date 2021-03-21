---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1bc658f2118f7b440855c727551d1f79429e72d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961325"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.termStore().groups("{groupId}")
    .buildRequest()
    .get();

```