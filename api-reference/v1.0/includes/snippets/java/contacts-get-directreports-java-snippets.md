---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 039a80030d5bb6df1228db08140fc3fcd6c25f2f
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638055"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionPage directReports = graphClient.contacts("{id}").directReports()
    .buildRequest()
    .get();

```