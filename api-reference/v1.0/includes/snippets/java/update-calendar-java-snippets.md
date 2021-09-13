---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: faca9558bf377ab854112aad5e641c7968dd095067f2e44bef9d40679cb76a56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = new Calendar();
calendar.name = "Social events";

graphClient.me().calendar()
    .buildRequest()
    .patch(calendar);

```