---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20c22f3b377b8dc48e905bf51141148d081c0b86f544cbf2d687e6cde9e8cdd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272191"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var masterCategories = await graphClient.Me.Outlook.MasterCategories
    .Request()
    .GetAsync();

```