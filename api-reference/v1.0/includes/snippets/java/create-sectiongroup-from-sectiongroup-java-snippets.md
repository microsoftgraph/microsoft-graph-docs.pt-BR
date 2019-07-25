---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d25f5d359c645dadc1a4d0f322ce898834b8fee
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882975"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroup sectionGroup = new SectionGroup();
sectionGroup.displayName = "Section group name";

graphClient.me().onenote().sectionGroups("{id}").sectionGroups()
    .buildRequest()
    .post(sectionGroup);

```