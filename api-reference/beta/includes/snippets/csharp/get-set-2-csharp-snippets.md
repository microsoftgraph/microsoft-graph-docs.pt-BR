---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce25000e7131c7bc812089b2b51ae987a552adc1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955399"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var set = await graphClient.TermStore.Sets["{termStore.set-id}"]
    .Request()
    .GetAsync();

```