---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78417d811fcbbec5987f8cbd2889120e4b471f617fb6fb85c9930d0ccfa64954
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/sites/{siteId}/drive')
    .get();

```