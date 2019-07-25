---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8529c3ebcf7d4257978d37f75fafc8c49c876162
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860206"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("10001")
    .buildRequest()
    .get();

```