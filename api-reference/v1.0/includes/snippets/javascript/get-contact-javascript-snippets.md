---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9032c25737de012a0a2c65926fbaaa34b89e4d0a441150c2e891b8251228bcf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contact = await client.api('/me/contacts/{id}')
    .get();

```