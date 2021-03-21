---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e084cb8106d1b5badadaeff5399929f0dd445608
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967933"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "displayName-value";
administrativeUnit.description = "description-value";
administrativeUnit.visibility = "visibility-value";

graphClient.directory().administrativeUnits("{id}")
    .buildRequest()
    .patch(administrativeUnit);

```