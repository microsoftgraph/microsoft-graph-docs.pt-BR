---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11ca2f2fff31706f4a8e7d1ed44a6ed54555cd2e787c94849ed2b56cbb925da6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899726"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let site = await client.api('/sites/{site-id}')
    .version('beta')
    .get();

```