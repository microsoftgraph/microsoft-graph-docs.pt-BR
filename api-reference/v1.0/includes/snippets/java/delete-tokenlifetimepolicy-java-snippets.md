---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22aa6ef457f26c1da8cc322d73a50074a6b4770cdf4f24d6dfe67de87e792c13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216223"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().tokenLifetimePolicies("{id}")
    .buildRequest()
    .delete();

```