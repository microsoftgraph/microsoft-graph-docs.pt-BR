---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 511d79baaacbde2ec23514843792d1cf4e6be686
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/projects')
    .version('beta')
    .get();

```