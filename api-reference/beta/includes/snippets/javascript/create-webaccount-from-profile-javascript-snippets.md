---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a7a23d40e4ac019fec1ccc484a934f4d4980a3a
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const webAccount = {
  description: "My Github contributions!",
  userId: "innocenty.popov",
  service: {
    name: "GitHub",
    webUrl: "https://github.com"
  }
};

let res = await client.api('/me/profile/webAccounts')
    .version('beta')
    .post(webAccount);

```