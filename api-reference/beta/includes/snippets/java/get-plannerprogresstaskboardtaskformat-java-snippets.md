---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28fc0d3d37fa914b9f97e64a749619d9ea7eed0b2060044cf8cd4be32c2cb05f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100806"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerProgressTaskBoardTaskFormat plannerProgressTaskBoardTaskFormat = graphClient.planner().tasks("{id}").progressTaskBoardFormat()
    .buildRequest()
    .get();

```