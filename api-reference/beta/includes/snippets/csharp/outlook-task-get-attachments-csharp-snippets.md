---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e1e2baa3f1eae97c7dee65077559f29e4cc463c0823ed3a230868bc701fb1a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Users["{user-id}"].Outlook.Tasks["{outlookTask-id}"].Attachments
    .Request()
    .GetAsync();

```