---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d3fb172e5c5b4adeee5d5f927069ede4b5a70da6e77bfc852387bbb2e6dedcd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214319"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plans = await graphClient.Groups["{group-id}"].Planner.Plans
    .Request()
    .GetAsync();

```