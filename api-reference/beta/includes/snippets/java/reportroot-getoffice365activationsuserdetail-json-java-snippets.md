---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 351586e0da06029771eacb2253c3d8b10902aa42
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873507"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ActivationsUserDetailCollectionPage getOffice365ActivationsUserDetail = graphClient.reports()
    .getOffice365ActivationsUserDetail()
    .buildRequest()
    .get();

```