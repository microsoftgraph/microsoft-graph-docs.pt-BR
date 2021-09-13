---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a48ad9c0c8136a58cd5c1e38a9f10685f7607f6e1afd4848f9d020b18d99818c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/me/schools')
    .get();

```