---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 172b4ea5fad101a592ab5bfc6db1e1caa27dda1d5a863d356006b493f869dbf1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213880"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages')
    .version('beta')
    .get();

```