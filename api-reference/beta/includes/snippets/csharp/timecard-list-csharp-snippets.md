---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7fada651ec31d9fdb254fb9bfa79fa869387ad77f77e807c6e19b2fc9911c2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeCards = await graphClient.Teams["{team-id}"].Schedule.TimeCards
    .Request()
    .Filter("state eq 'clockedOut'")
    .Top(2)
    .GetAsync();

```