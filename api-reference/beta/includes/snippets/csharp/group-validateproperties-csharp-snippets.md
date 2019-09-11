---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e11721228461b82cdcf8ed6f108630f5f97ff705
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845850"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Myprefix_test_mysuffix";

var mailNickname = "Myprefix_test_mysuffix";

var onBehalfOfUserId = Guid.Parse("onBehalfOfUserId-value");

await graphClient.Groups["{id}"]
    .ValidateProperties(displayName,mailNickname,onBehalfOfUserId)
    .Request()
    .PostAsync();

```