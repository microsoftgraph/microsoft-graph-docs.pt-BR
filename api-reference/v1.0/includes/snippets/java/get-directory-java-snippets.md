---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f48465bc8c794a31af7ab7f8034ec5a2cddde37f158de0cdec8381c6e07b7d3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330061"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .get();

```