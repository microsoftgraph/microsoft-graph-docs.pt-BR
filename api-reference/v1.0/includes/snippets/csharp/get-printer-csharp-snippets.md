---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11d18a0a1c43dc70b736ce64ed529b1df031c3997c927d942e26c671988e5b37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printer = await graphClient.Print.Printers["{printer-id}"]
    .Request()
    .GetAsync();

```