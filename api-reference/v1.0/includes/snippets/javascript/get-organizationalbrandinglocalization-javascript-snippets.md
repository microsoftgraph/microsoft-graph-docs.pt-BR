---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26602ac2c9e1e85fd9c9a01a6a65ff673928f266
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let organizationalBrandingLocalization = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR')
    .get();

```