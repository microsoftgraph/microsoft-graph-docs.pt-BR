---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 727bb30d45603b53f823be1284fd1bfc560cbf5bf68bc62cd1429eed04c23cff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157248"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.devices("{id}").registeredOwners("{id}").reference()
    .buildRequest()
    .delete();

```