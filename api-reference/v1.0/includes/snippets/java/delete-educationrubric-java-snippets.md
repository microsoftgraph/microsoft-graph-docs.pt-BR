---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f32ff59b9c1dd34164eb22f0f4a1c76c508fb9089b8a9de2542bca0e27fd984
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102015"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().me().rubrics("ceb3863e-6912-4ea9-ac41-3c2bb7b6672d")
    .buildRequest()
    .delete();

```