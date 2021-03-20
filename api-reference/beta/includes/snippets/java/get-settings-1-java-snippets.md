---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32114b75c9c60a940ed07399059e1d4cc08ebb7a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946520"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectorySettingCollectionPage settings = graphClient.settings()
    .buildRequest()
    .get();

```