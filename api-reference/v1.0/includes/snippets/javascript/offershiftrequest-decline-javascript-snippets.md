---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25e4da31505f6aeecb049b50fb481b162b7553937be0b704fe167564e0cd4081
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217006"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: 'Sorry, you can\'t offer this shift.'
};

await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline')
    .post(decline);

```