---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d890bb3c0ad7d782baca14d6ca483693478864a1ade1ad8a8a21acc8b9bad6a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406865"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffRequests = await client.api('/teams/{teamId}/schedule/timeOffRequests')
    .get();

```