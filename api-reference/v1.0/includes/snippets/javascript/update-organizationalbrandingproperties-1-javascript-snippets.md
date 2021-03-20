---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca14c349434bcfb3ae65f39bb26f729a1a486086
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBranding = {
    signInPageText: 'Default',
    usernameHintText: 'DefaultHint'
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding')
    .update(organizationalBranding);

```