---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7774ee2cafc267b42262a2e74f129f65b8f06596
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/certifications')
    .version('beta')
    .get();

```