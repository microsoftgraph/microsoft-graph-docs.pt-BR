---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 560d051f65ef817b4be6df529bb69b00d470b73a
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f')
    .version('beta')
    .delete();

```