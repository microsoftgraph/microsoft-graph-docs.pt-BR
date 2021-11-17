---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab41ba53297f248dc1bbd36cbe9cef21ff559bf87baf6222babebbbe0f34951f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/users/delta')
    .version('beta')
    .get();

```