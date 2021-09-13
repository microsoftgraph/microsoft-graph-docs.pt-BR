---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4df51c618302afa5858a91dea73665d2761e18de9afd7ec933556feff572a81f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let domain = await client.api('/domains/contoso.com')
    .get();

```