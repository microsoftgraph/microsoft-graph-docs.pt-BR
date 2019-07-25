---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee81bba1f7d60bae206e6d0b47691224c6d241db
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855782"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.education().schools("2961761D-8094-4183-A9F6-8E36E966C7D9").administrativeUnit()
    .buildRequest()
    .get();

```