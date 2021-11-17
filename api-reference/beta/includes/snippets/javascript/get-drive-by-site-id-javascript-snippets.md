---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f831ab171befeb7e26452582cca3fa9edcbcce09413ff766c67ff0e2baa52fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/sites/{siteId}/drive')
    .version('beta')
    .get();

```