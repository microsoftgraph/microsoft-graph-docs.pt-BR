---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df667e3e22f0fad71a18fa72d25385296fc98071
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739958"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{class-id}"]
    .Request()
    .DeleteAsync();

```