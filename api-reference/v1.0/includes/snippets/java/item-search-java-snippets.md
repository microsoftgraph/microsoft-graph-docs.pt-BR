---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba76a050dcd130f2d0ba415a13074e4b018b9290
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983076"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemSearchCollectionPage search = graphClient.me().drive().root()
    .search("Contoso Project")
    .buildRequest()
    .get();

```