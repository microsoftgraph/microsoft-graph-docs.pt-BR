---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de5a27a289773683079cf570b39c35e295991d9a79a4f5fe0be32b83cebe630d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275001"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = graphClient.teams("893075dd-2487-4122-925f-022c42e20265")
    .buildRequest()
    .get();

```