---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a6e8308ce4d3b3022ce52a747c71942d0986003
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932632"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bundles = await graphClient.Drive.Bundles
    .Request()
    .GetAsync();

```