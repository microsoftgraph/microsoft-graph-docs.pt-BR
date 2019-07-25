---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a46a279e3ba7fb7910fb4c7670e60df54eba7130
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888067"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.me().drive().items("{item-id}").children()
    .buildRequest()
    .expand("thumbnails")
    .get();

```