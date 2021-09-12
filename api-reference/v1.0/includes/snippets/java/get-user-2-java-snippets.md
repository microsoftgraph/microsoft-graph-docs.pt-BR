---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6652cb77a265162af0d50c5e29419232bac947fd1e688ca522cdbe4bab36c279
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214262"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.users("{id | userPrincipalName}")
    .buildRequest()
    .select("displayName,givenName,postalCode")
    .get();

```