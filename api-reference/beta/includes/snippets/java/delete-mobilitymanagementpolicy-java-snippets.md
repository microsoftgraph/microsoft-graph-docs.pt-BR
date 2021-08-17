---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b3bafce06cb8d8d7c928e9b973ced6066b82e07
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368800"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().mobileAppManagementPolicies("ab90bacf-55a3-4a3e-839a-aa4b74e4f020")
    .buildRequest()
    .delete();

```