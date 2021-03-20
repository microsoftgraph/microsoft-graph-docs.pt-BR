---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e959d20228461b2a041ef3598178521af9cfd841
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948866"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.Print.Connectors
    .Request()
    .GetAsync();

```