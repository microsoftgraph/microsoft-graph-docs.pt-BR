---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70e913fe1dd6bc0c476defc79d00116187ec3c72
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875410"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProgramCollectionPage programs = graphClient.programs()
    .buildRequest()
    .get();

```