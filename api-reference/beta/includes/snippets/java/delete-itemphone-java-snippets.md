---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5c91c659c593c4973bac3f37e37f1be923b49a42e6aed750694394e8b5d038d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275039"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{userId}").profile().phones("{itemPhoneId}")
    .buildRequest()
    .delete();

```