---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7471dc28e411057411a091fa19a957a7eaee948cef0d3212686e0b14d9ea4cb9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272554"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var outlookTaskFolder = new OutlookTaskFolder
{
    Name = "Charity work"
};

await graphClient.Me.Outlook.TaskFolders["{outlookTaskFolder-id}"]
    .Request()
    .UpdateAsync(outlookTaskFolder);

```