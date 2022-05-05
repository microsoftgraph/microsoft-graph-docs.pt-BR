---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3f1ec2d929ca062ff6860b318d7d7187229893d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205689"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MicrosoftApplicationDataAccessSettings microsoftApplicationDataAccessSettings = graphClient.organization("{organizationId}").settings().microsoftApplicationDataAccess()
    .buildRequest()
    .get();

```