---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c675d10702d9cb7b8fb9dc771ddff28edd6162f5a592eecb0ee940101b1fc02a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216113"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callRecord = await graphClient.Communications.CallRecords["{callRecords.callRecord-id}"]
    .Request()
    .Expand("sessions($expand=segments)")
    .GetAsync();

```