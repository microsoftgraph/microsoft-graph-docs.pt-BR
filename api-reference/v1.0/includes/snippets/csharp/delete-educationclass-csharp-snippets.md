---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df667e3e22f0fad71a18fa72d25385296fc98071
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466716"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{class-id}"]
    .Request()
    .DeleteAsync();

```