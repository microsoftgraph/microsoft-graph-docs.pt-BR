---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4442d89ec0008dd9470b89b0aa63aa441d99b9f4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888393"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{class-id}")
    .buildRequest()
    .delete();

```