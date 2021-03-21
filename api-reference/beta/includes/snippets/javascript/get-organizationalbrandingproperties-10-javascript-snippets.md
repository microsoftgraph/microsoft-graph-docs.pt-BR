---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1375e4c50ff3a9943095f04ae67221715721ab4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText')
    .version('beta')
    .get();

```