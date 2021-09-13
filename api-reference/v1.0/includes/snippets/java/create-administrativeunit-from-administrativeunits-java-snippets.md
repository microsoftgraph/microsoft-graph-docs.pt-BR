---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19fb0f84038adbaa1b4bada62c1174755630a38b6e77de7e63fe43c66cb33193
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407551"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "Seattle District Technical Schools";
administrativeUnit.description = "Seattle district technical schools administration";
administrativeUnit.visibility = "HiddenMembership";

graphClient.directory().administrativeUnits()
    .buildRequest()
    .post(administrativeUnit);

```