---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d19100b7982c14db11b48c53c81bbd05e1e985b5
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBrandingLocalization = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR')
    .version('beta')
    .get();

```