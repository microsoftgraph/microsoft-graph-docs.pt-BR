---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd717ed62dc76d415d4bed3b7d639708d47030fe5e6e92dd0f6ac329123e49cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157017"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationalActivity = await client.api('/me/profile/educationalActivities/{id}')
    .version('beta')
    .get();

```