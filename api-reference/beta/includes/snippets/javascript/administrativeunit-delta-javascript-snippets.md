---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7388e94981cbecaf22c29ccc08b7a21e74939f0c080e52fd3e185e1817cd2f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898099"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/administrativeUnits/delta')
    .version('beta')
    .get();

```