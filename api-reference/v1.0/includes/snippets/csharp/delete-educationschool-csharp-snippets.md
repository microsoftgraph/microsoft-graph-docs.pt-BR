---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6fa6bcf334d47b90b18e90969d049bf19672292
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466713"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{school-id}"]
    .Request()
    .DeleteAsync();

```