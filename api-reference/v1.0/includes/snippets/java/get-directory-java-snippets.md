---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3b18d39708d1fda22577c1e6fd9c24b569f02c3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883292"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .get();

```