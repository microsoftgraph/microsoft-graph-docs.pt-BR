---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f04739e606cc20a5ca67a24b937d2a330d847c4fecb2d611ac6b304c95d1d935
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329376"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

StringCollectionPage responsibilities = graphClient.customRequest("/me/responsibilities", StringCollectionPage.class)
    .buildRequest()
    .get();

```