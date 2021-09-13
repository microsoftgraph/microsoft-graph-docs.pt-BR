---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e92b75b96277c267a5ca29b80c0ef4693a681a9f6db2e926671ae6663397f944
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217590"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublicationCollectionPage publications = graphClient.me().profile().publications()
    .buildRequest()
    .get();

```