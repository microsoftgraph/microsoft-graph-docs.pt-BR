---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0986ffbfd92d3e2e560dc8a3d4a0f7277a46acc461542e2afc57c7711e6bac5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Planner.Rosters["{plannerRoster-id}"]
    .Request()
    .DeleteAsync();

```