---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a96b9370696c3f629edd0420a7fe999b9e9ee8d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137464"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionPage internalSponsors = graphClient.identityGovernance().entitlementManagement().assignments("{accessPackageAssignmentId}").target().connectedOrganization().internalSponsors()
    .buildRequest()
    .get();

```