---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37c5078d8b28a9dc603ce1ffe6e9cbb43556ce5e1ebd9d7715fedbae59cf39e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffRequests = await client.api('/teams/{teamId}/schedule/timeOffRequests')
    .version('beta')
    .get();

```