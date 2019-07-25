---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00bbf388d11d466249fcb7fa92fb390249881b22
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861614"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.groups("{groupId}").drive()
    .buildRequest()
    .get();

```