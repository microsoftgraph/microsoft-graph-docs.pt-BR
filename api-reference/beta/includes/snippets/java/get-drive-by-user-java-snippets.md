---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3524c3d143bced8da2f9d094dbc8393bedd58fc2c917590649b425d0ffc957c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100856"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.users("{idOrUserPrincipalName}").drive()
    .buildRequest()
    .get();

```