---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97168e01b407ba752f024936a1c5579a1cea1a0e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945808"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shiftPreferences = await graphClient.Users["{user-id}"].Settings.ShiftPreferences
    .Request()
    .GetAsync();

```