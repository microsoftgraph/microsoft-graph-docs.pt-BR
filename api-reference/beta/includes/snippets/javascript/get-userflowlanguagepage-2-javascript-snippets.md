---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a80bc3ce11ae22534c65fa154a33703297490ac03af17fe5c08a5fb9590e952e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100324"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let overridesPages = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages')
    .version('beta')
    .get();

```