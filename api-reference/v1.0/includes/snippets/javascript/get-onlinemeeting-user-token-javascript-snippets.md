---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24f64d69ad9b5e416181e9fb7aae35244bdb7bfe289c5f15af880d54067bf791
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onlineMeeting = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy')
    .version('beta')
    .get();

```