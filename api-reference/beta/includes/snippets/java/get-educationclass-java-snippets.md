---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd82be27683cb6bd824b33b446baae2509fac15c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860630"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = graphClient.education().classes("11023")
    .buildRequest()
    .get();

```