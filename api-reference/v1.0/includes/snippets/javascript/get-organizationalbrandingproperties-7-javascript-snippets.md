---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 989b1c400299f794d2d42a856a73e5edc30a5c0a56015a5022c3577762e8d27b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157553"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBrandingLocalization = {
    backgroundColor: '#00000F',
    id: 'fr'
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations')
    .post(organizationalBrandingLocalization);

```