---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad701bbdfc11f5dbcd563eaa9e5b620186fdc89cf9e2284e9133c47958402bbf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = graphClient.servicePrincipals("{id}")
    .buildRequest()
    .get();

```