---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a36a9359135ff37aa7117f7bf2df3d872fdd83111ddde5f7ba782b5537dcca0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157541"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printJob = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Request()
    .Expand("tasks")
    .GetAsync();

```