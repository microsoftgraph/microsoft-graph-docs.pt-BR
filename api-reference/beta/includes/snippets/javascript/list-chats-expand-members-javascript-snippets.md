---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 266031ff977b85d447188ce9d8d9ac620fb0d1f19a48280128381ca483f9c6c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let chats = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats')
    .version('beta')
    .expand('members')
    .get();

```