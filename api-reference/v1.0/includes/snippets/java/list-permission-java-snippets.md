---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b345bcb0070c860718ef9014b070810c57956b6c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176823"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPermissionCollectionPage permissions = graphClient.sites("{sitesId}").permissions()
    .buildRequest()
    .get();

```