---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aba55282a5292a4472ce1f9647da430d534416bb
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const webAccount = {
  webUrl: "https://github.com/innocenty.popov"
};

let res = await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .update(webAccount);

```