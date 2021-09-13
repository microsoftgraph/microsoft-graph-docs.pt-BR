---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6128a86a87671711814048818b18d428ad5922b809f030eb9b60696ddfc2181
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275643"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let offerShiftRequests = await client.api('/teams/{teamId}/schedule/offerShiftRequests')
    .get();

```