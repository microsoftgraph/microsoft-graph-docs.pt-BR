---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5495328a885866a3b898dd580be2aaecd07ac034572fdb5015b0baa0a7f93313
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217502"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupSettings["{groupSetting-id}"]
    .Request()
    .DeleteAsync();

```