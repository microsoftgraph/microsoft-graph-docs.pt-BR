---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dc5e3cff96bd7fcf5bb8b8b9e889d679cfa25538aacd6ca3753641949176d8a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShift = await graphClient.Teams["{team-id}"].Schedule.OpenShifts["{openShift-id}"]
    .Request()
    .GetAsync();

```