---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 540d48bdd7d43eff2343d1fdcc08608a96704f198cd2ecec6d3509dba6f1c07c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttribute = {
  displayName: 'Hobby',
  description: 'Your hobby',
  dataType: 'string',
};

await client.api('/identity/userFlowAttributes')
    .post(identityUserFlowAttribute);

```