---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db17996943696b075a97845f06766399a97a66c36ed59599cc6d9c6c7a28ca98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rejectedSenders = await graphClient.Groups["{group-id}"].RejectedSenders
    .Request()
    .GetAsync();

```