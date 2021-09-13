---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9293577f0d0c97554591fe054d39a69aee47a31a67b04a433c2f357ca0c11bb5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215271"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/schools')
    .get();

```