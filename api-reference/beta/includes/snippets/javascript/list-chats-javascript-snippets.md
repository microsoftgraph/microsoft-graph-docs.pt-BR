---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 415ed5a902e7763e0cea8539fe6857482bfd5f3d8eec0a547437394f146b0074
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158042"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chats = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats')
    .version('beta')
    .get();

```