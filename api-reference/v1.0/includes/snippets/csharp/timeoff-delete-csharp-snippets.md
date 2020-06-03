---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3be0f4ffaa46cf424b5101cccb8667c7e9d0a02f
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44218044"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Schedule.TimesOff["{timeOffId}"]
    .Request()
    .DeleteAsync();

```