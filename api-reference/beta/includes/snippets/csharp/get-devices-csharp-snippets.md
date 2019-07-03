---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9736f77673ba3109534e651a587fd3641c173d5b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var devices = await graphClient.Devices
    .Request()
    .GetAsync();

```