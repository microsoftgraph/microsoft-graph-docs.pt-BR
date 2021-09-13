---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1854300d6524131d967cc5a372c1fda50038ac7fd9933db74430b139513a3c48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272383"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReason = await graphClient.Teams["{team-id}"].Schedule.TimeOffReasons["{timeOffReason-id}"]
    .Request()
    .GetAsync();

```