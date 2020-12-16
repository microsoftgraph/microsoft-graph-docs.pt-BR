---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a222a72d9ae3823e2b9df007bce0566772610c2
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/channels/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/tabs')
    .version('beta')
    .expand('teamsApp')
    .get();

```