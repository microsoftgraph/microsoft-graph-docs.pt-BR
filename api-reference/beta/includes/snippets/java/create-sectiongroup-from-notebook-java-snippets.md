---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 851021b071fe66cb8df8d090d8928714b6830c65
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967704"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroup sectionGroup = new SectionGroup();
sectionGroup.displayName = "Section group name";

graphClient.me().onenote().notebooks("{id}").sectionGroups()
    .buildRequest()
    .post(sectionGroup);

```