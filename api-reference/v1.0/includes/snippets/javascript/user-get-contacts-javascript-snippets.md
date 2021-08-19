---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbfbd79cee395d75288841f6c19800a1982d5321d76cadd91722a2a8adc34f10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272890"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contacts = await client.api('/me/contacts')
    .get();

```