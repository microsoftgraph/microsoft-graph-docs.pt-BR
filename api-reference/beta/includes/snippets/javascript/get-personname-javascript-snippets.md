---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 962dc48024f4a152202aedfa5eab25a8db8c88b62d79d4ec69f7680ed19b76a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personName = await client.api('/me/profile/names/{id}')
    .version('beta')
    .get();

```