---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2c11b8021dbb222f38109c66ad4650ec84dd81de
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888070"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IThumbnailSetCollectionPage thumbnails = graphClient.me().drive().items("{item-id}").thumbnails()
    .buildRequest()
    .get();

```