---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03a62fc655cbbdab147da727cd99a0246a542319
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.MasterCategories["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"]
    .Request()
    .DeleteAsync();

```