---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2cdf2041f31f6a5ab20bd74d25579177f5a9807d
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933775"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var call = await graphClient.App.Calls["{id}"]
    .Request()
    .GetAsync();

```