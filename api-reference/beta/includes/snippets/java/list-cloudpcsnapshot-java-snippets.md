---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 530677126a5d365280b63c4885b02ccf0801e4fd
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335322"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcSnapshotCollectionPage snapshots = graphClient.deviceManagement().virtualEndpoint().snapshots()
    .buildRequest()
    .get();

```