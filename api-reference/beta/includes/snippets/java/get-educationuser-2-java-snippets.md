---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0f1ca28bb88254482f2a0e047766a92c6a160e5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951133"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = graphClient.education().users("13012")
    .buildRequest()
    .get();

```