---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afc0cbdd57e5fc291f3aef063b6930cd737d032f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855458"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = graphClient.agreements("'id'")
    .buildRequest()
    .expand("files")
    .get();

```