---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af74826f7bac497c9b9090195d69cabd4a3eb5eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980221"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = graphClient.education().classes("{id}").assignmentSettings()
    .buildRequest()
    .get();

```