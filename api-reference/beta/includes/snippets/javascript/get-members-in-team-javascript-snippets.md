---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d13d825089f0eb14d1a8d2d2014521a29ac0d655dbd72abed511ab6863e59f85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159621"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .version('beta')
    .get();

```