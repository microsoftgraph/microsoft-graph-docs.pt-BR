---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53978bf17d3d661707693e5d32fa862af7f74a4cefda8f4c6b9f4492cdff0127
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage following = graphClient.me().drive().following()
    .buildRequest()
    .get();

```