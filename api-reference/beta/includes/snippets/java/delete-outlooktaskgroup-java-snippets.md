---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e95d67d224600bd647b0fd9ece5dad572d8938cbf87884fe8450e35fa15ceba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215354"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=")
    .buildRequest()
    .delete();

```