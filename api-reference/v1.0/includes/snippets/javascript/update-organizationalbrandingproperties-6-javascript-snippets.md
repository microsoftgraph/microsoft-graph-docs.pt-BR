---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1521719ea13abd02a1050655fb6929d78ab062205a4e5f3c269ea346e5eabc5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organizationalBrandingLocalization = {
    backgroundColor: '#00000F',
    signInPageText: 'fr'
};

await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr')
    .update(organizationalBrandingLocalization);

```