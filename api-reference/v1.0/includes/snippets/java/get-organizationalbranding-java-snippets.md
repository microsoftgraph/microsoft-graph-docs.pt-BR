---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1d601b3637ba35a363fcfe96a2d5fb4c10f3f661
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562724"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Accept-Language", "0"));

OrganizationalBranding organizationalBranding = graphClient.organization("84841066-274d-4ec0-a5c1-276be684bdd3").branding()
    .buildRequest( requestOptions )
    .get();

```