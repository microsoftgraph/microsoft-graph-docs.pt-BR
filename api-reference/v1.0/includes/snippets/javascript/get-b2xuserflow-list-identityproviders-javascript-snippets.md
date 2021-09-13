---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 300e208021ab82d2a4103c16d7ca055c75e842d3acd45894c4ab8547ab82c870
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327163"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identity/b2xUserFlows/B2X_1_Partner/identityProviders')
    .get();

```