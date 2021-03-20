---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4103de7a14fed828dfc70da904e84c53e80d65ba
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stream = <Image>;

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo')
    .version('beta')
    .put(stream);

```