---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0883cde96f8a29610fee10f633535b17e7ffde4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951626"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Teachers["{educationUser-id}"]
    .Request()
    .DeleteAsync();

```