---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aac5d2876cdced2da12dc24376fe56b0b6f591ed6f21fe84e3c4e5a89f2fc1d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let allowedUsers = await client.api('/print/shares/{id}/allowedUsers')
    .version('beta')
    .get();

```