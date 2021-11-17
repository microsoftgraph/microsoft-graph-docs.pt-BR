---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3976266d257fc80992da004bdec7c21c3bb60c817dfecee1a43f7fe63cc637eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100212"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applicationTemplates = await graphClient.ApplicationTemplates
    .Request()
    .GetAsync();

```