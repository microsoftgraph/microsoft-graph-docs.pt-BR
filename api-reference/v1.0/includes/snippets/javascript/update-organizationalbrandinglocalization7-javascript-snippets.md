---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9355d4ae19ba86c9ddf33a087096baa912556dc5
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996872"
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
    .update(organizationalBrandingLocalization);

```