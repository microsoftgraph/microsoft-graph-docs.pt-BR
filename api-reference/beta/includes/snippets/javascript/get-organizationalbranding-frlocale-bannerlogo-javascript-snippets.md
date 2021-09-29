---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 817b758bb36027c517998831986d4cc81953cd59
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/default/bannerLogo')
    .version('beta')
    .get();

```