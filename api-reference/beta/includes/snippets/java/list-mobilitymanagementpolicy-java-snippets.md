---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7156c5237522fe43a8dd44095ba5a118e7bbb897
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368797"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MobilityManagementPolicyCollectionPage mobileDeviceManagementPolicies = graphClient.policies().mobileDeviceManagementPolicies()
    .buildRequest()
    .get();

```