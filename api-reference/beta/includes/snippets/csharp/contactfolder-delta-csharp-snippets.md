---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a37bf299e71cc57642ccca9b4f11178a4e1f3042
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517680"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders.Delta()
    .Request()
    .GetAsync();

```