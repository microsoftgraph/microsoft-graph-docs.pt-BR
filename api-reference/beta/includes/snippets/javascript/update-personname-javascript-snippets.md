---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 255f2cc57c44013acf263c25b2f928b67fe9deef
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821148"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personName = {
  nickname: "Kesha"
};

let res = await client.api('/me/profile/names/{id}')
    .version('beta')
    .update(personName);

```