---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9317774d5ae7e9f0564b75c0c24e72a7991522b9a0f1929b476f063358b30f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326890"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{contactFolder-id}"].Contacts
    .Delta()
    .Request()
    .Select("displayName")
    .GetAsync();

```