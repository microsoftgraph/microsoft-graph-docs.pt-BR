---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8a585691b516cf13a824ff858d36c562095f941c528d0d316c79e177c3ad242
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredDevices = await client.api('/me/registeredDevices')
    .version('beta')
    .get();

```