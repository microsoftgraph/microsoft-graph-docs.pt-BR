---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e61ddc2ef6e6b6013745602caf380495ec9b25f1
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179558"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionPage users = graphClient.users()
    .buildRequest()
    .filter("startswith(displayName,'Eric')")
    .select("displayName,signInActivity")
    .get();

```