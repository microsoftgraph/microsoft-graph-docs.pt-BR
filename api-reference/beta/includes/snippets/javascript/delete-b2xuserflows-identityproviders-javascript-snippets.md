---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f373520f99db57ec2b44463f7eb08935b2ead5fa
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/identityProviders/Facebook-OAUTH/$ref')
    .version('beta')
    .delete();

```