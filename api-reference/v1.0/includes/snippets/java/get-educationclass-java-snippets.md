---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7883568e6d4d90a02388cc609d6cbf24822a999f
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474992"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClass educationClass = graphClient.education().classes("{educationClassId}")
    .buildRequest()
    .get();

```