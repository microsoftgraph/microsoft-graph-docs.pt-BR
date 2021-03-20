---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23ec8e632cf3a18b96355bd602164d7c335f9570
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950660"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.Print.Shares["{printerShare-id}"].Jobs
    .Request()
    .GetAsync();

```