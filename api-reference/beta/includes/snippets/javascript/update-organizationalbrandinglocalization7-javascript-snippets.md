---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1281e4ee2d1baa5f3cbf24aa94c5dc03ddd61cff
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBrandingLocalization = {
    signInPageText: 'Welcome to Contoso France.',
    usernameHintText: ' '
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR')
    .version('beta')
    .update(organizationalBrandingLocalization);

```