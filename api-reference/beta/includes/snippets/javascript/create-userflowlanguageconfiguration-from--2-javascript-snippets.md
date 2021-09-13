---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f90a15cd9f1870206753d4e2245cc10607e4db63249848a172f326f41debcce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213865"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userFlowLanguageConfiguration = {
  isEnabled: false
};

await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES')
    .version('beta')
    .put(userFlowLanguageConfiguration);

```