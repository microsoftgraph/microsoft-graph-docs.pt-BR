---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: beb7638d07886d79c83c39a636c3ceb879557d5a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let federatedIdentityCredentials = await client.api('/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/')
    .version('beta')
    .get();

```