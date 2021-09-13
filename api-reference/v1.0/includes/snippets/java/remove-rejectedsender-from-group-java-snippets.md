---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b201d3f927c91e3968d08120074aca27ecb02fac05634373bcef7b555e45c7af
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327700"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").rejectedSenders().references()
    .buildRequest()
    .delete();

```