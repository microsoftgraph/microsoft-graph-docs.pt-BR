---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45351bbeb9a2a17e210a7c2c5f461b0d802ccac00812f7a8bbf0ff2c26a0eacd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326996"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.groups("45b7d2e7-b882-4a80-ba97-10b7a63b8fa4")
    .buildRequest()
    .get();

```