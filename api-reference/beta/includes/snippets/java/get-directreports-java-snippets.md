---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4ac6739599961ea857895ab64ed0290d15870c61d813479bca53a7709dca50b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329618"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage directReports = graphClient.me().directReports()
    .buildRequest()
    .get();

```