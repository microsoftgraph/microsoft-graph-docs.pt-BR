---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 821383bccf53e7ba91b3200d25e2620b42c7be04616506f99d6e64bbdad1bcfc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327451"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = await graphClient.Me.Contacts["{contact-id}"]
    .Request()
    .GetAsync();

```