---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5db0909ad65863247ba369bf0ad1ba7b838a330
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873955"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage search = graphClient.me().drive().root()
    .search("Contoso Project")
    .buildRequest()
    .get();

```