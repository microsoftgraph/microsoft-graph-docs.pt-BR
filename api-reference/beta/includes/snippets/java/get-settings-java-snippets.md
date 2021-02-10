---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32114b75c9c60a940ed07399059e1d4cc08ebb7a
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179144"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectorySettingCollectionPage settings = graphClient.settings()
    .buildRequest()
    .get();

```