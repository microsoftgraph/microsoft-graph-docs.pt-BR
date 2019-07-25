---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7023b2fc56fef26c5a1725e44901e1ece2fe9be
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873438"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ActiveUserDetailCollectionPage getOffice365ActiveUserDetail = graphClient.reports()
    .getOffice365ActiveUserDetail('D7')
    .buildRequest()
    .get();

```