---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0b537d9ae32a13ba443f9f503fb3fe14ed0ea11e35d167e7ebff89b7eaca0f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214554"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}").mentions("{id}")
    .buildRequest()
    .delete();

```