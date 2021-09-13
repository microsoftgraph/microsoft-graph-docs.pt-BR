---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da014e4170b2037432193a8c1a76fd6a8a48c12f6c90e904da9be122140d3cb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157317"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().activities("{activity-id}")
    .buildRequest()
    .delete();

```