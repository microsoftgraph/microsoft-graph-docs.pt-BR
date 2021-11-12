---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad4cfdfb37555332b7201a0f548582a51b62ac8fb7c958a3eace058ae57e2966
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898090"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .GetAsync();

```