---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47acdf174270240f51c985df3925640fa3036c1ad7f6b0f87e4db3d1f36d7162
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/calendar')
    .version('beta')
    .delete();

```