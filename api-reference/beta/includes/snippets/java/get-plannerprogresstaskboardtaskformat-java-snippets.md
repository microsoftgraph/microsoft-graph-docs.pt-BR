---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04f9e92cafa8233a180d7163d971e678fdb2dd30
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977978"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = graphClient.planner().tasks("{id}").progressTaskBoardFormat()
    .buildRequest()
    .get();

```