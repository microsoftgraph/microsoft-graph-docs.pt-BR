---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b27f598988caf220f03889a959dc423bcda65bb7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862242"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("{id}")
    .buildRequest()
    .get();

```