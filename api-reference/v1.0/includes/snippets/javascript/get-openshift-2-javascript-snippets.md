---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 136b5a10806afe6f03624d22a8d91d813242590bdf68286fdd972ff6839ade4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158096"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let openShifts = await client.api('/teams/{id}/schedule/openShifts')
    .get();

```