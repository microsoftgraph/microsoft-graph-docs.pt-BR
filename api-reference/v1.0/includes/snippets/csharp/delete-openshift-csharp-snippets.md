---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73e84873b25b7e66b32e66e3bb2e2613c449e139
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217203"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Schedule.OpenShifts["OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"]
    .Request()
    .DeleteAsync();

```