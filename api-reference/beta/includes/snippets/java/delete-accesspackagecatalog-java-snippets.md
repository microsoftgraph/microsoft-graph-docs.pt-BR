---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6499ce5b57b8892622deaca8e9c9c076587ab9b7674feb95c4be146caa2b4c15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156601"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs("{id}")
    .buildRequest()
    .delete();

```