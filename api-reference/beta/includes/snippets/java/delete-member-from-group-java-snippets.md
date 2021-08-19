---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d37be3257c2409a9496ab635e99b9e40fcc73b86efd433718102a98bb962287b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216591"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{group-id}").members("{directory-object-id}").reference()
    .buildRequest()
    .delete();

```