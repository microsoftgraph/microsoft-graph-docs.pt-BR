---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af00933c05971c7f18c8cb4841adba996344e8ce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893849"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Stream Stream = graphClient.customRequest("/me/onenote/resources/{id}/content", Stream.class)
    .buildRequest()
    .get();

```