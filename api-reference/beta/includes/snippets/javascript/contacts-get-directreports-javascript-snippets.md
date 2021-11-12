---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 129d888e5af71850ab1573a0bc7cdb0df64f2969cd17c47d8d62ee513a027a85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directReports = await client.api('/contacts/{id}/directReports')
    .version('beta')
    .get();

```