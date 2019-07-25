---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc280236aa5170886c5f2778f31214bf72cc0264
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709276"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var businessFlowTemplates = await graphClient.BusinessFlowTemplates
    .Request()
    .GetAsync();

```