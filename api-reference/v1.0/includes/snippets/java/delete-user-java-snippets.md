---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53ad05e9d766b28bd4e5e91a2b403e940fecb3c0e356b221c0867a30cb2bab67
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102191"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{user-id}")
    .buildRequest()
    .delete();

```