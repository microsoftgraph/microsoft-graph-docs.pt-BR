---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a043cc07950b0eedd12c8afaed6534ccccb3c7b6ec73b375cfc20f6a7138a46f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159642"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().interests("{id}")
    .buildRequest()
    .delete();

```