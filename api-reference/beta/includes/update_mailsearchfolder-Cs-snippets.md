---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a8541c506be09c6aeed64673e2bfd14642ddfa8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274876"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    FilterQuery = "contains(subject, 'Analytics')"
};

await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .UpdateAsync(mailFolder);

```