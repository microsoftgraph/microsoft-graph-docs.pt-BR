---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 066d81e6d420828131eea7d502177ca1d2f954b6ba8a207804b45038eb4d049d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156328"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var noncustodialDataSources = await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].NoncustodialDataSources
    .Request()
    .GetAsync();

```