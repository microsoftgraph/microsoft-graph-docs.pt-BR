---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09c5db77df5cb77970105daffb869469825295b49b2124546c93d10f465f6e71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShiftChangeRequests = await client.api('/teams/{id}/schedule/openShiftChangeRequests')
    .get();

```