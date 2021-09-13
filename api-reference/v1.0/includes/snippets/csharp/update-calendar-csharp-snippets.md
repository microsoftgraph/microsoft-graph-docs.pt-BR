---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9cfb6b4ca2a1c03904bf376c286dc238327e012e6d053a72036f52895adc7df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = new Calendar
{
    Name = "Social events"
};

await graphClient.Me.Calendar
    .Request()
    .UpdateAsync(calendar);

```