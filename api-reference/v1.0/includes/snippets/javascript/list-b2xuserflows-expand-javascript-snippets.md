---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb586989d5bc13581e2c1979e01754bee59f3e4066e82ca7c879ce34927bc282
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2xUserFlows = await client.api('/identity/b2xUserFlows')
    .expand('identityProviders')
    .get();

```