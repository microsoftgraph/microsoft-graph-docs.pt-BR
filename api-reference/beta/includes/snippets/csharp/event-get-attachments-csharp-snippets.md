---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 783ded2727451ce3a79d1dcbbecdec8355d20d0a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859553"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Me.Events["{id}"].Attachments
    .Request()
    .GetAsync();

```