---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53a32faa498230ea2658dae87af96a9945858895
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let _boolean = await client.api('/teams/{0fddfdc5-f319-491f-a514-be1bc1bf9ddc}/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/doesUserHaveAccess(userId='6285581g-484b-4845-9e01-60667f8b12ae')')
    .version('beta')
    .get();

```