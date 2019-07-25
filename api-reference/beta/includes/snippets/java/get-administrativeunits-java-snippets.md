---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa71711a82cecc7dae13317280c156dc80450912
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855808"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAdministrativeUnitCollectionPage administrativeUnits = graphClient.administrativeUnits()
    .buildRequest()
    .get();

```