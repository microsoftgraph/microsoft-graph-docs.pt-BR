---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21e00945df55e27370c0f8718d97e5fcd87441a271f605e3421c2ce517d99752
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214653"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .delete();

```