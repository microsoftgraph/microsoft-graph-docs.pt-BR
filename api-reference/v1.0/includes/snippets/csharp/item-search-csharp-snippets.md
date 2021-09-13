---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32c293636e20e1aa84cb18d3639129b5a498be027bcf78f2000564304cd2a7e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899331"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Root
    .Search("Contoso Project")
    .Request()
    .GetAsync();

```