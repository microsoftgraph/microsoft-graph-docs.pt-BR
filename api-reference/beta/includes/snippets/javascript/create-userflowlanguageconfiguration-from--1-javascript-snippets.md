---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d955db760d1c273c876bb3623f4e4a920176165f2b9829242f4001c67492c49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userFlowLanguageConfiguration = {
  id: 'es-ES',
  isEnabled: true
};

await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES')
    .version('beta')
    .put(userFlowLanguageConfiguration);

```