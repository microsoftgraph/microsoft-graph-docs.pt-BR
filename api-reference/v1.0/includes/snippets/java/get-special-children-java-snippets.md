---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2eed18d35f7cd0a15785f41da1ca34f252d314f9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979441"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemCollectionPage children = graphClient.me().drive().special("{special-folder-name}").children()
    .buildRequest()
    .get();

```