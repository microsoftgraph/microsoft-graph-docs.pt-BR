---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a53f033b32182626a24080a77f2ece5ec2ceff6ae6d9b1827c3ebefedcf0124c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217319"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().emails("{id}")
    .buildRequest()
    .delete();

```