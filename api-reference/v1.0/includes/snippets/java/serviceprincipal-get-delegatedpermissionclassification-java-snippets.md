---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c04560085b56855d6c5aa8c03610872280b38796
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DelegatedPermissionClassificationCollectionPage delegatedPermissionClassifications = graphClient.servicePrincipals("{id}").delegatedPermissionClassifications()
    .buildRequest()
    .get();

```