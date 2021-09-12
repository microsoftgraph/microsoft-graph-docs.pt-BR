---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6c36cc35469aa4f329fe9f5f8b082e3e094f5127f3d9504e55015fd8a0e45c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159776"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAddressCollectionPage addresses = graphClient.me().profile().addresses()
    .buildRequest()
    .get();

```