---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bac3a373f669abc9d239c8e032488af2e49b1400a24f3e7497a587d7a22be569
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271809"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let certifications = await client.api('/me/profile/certifications')
    .version('beta')
    .get();

```