---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: def2195eb462edf2c0add8a362794768f1759f6f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336353"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{id}";

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}").internalSponsors().references()
    .buildRequest()
    .post(directoryObject);

```