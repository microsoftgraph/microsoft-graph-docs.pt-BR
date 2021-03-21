---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06054ef40ba1a54878f3057b3789380fabefa1b4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983367"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.administrativeUnits("{id}")
    .buildRequest()
    .get();

```