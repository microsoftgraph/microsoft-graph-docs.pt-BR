---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0e497b72e6ea2627b4842c8f33fb8884ae652fcc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477202"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessParticipantActivityMinuteCounts = await graphClient.Reports.GetSkypeForBusinessParticipantActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```