---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da999d393b99925c6c7339be55301e176810565224c7669009bb1a251f9338c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedDevices = await client.api('/me/ownedDevices')
    .version('beta')
    .get();

```