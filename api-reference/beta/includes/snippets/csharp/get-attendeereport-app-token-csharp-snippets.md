---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 149587707c7c0fa4637f088bfee82b721b169460
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Users["{user-id}"].OnlineMeetings["{onlineMeeting-id}"].AttendeeReport
    .Request()
    .GetAsync();

```