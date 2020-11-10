---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8529c3ebcf7d4257978d37f75fafc8c49c876162
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955592"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = graphClient.education().schools("10001")
    .buildRequest()
    .get();

```