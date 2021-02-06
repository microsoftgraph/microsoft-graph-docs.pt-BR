---
title: tipo optionalClaims
description: Declara as declarações opcionais solicitadas por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: d50b514fa29cf99f22bb42238ac9d6a66126ab53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132653"
---
# <a name="optionalclaims-resource-type"></a>Tipo de recurso optionalClaims

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Declara as declarações opcionais solicitadas por um aplicativo. Um aplicativo pode configurar declarações opcionais a serem retornadas em cada um dos três tipos de tokens (token de ID, token de acesso, token SAML 2) que ele pode receber do serviço de token de segurança. Um aplicativo pode configurar um conjunto diferente de declarações opcionais a serem retornadas em cada tipo de token. A propriedade optionalClaims do [aplicativo é](application.md) um **objeto optionalClaims.**

Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações desejam em tokens enviados ao aplicativo pelo serviço de token de segurança da Microsoft. Confira [fornecer declarações opcionais ao aplicativo Azure AD](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|idToken|[coleção optionalClaim](optionalclaim.md)| As declarações opcionais retornadas no token de ID JWT. |
|accessToken|[coleção optionalClaim](optionalclaim.md)| As declarações opcionais retornadas no token de acesso JWT. |
|saml2Token|[coleção optionalClaim](optionalclaim.md)| As declarações opcionais retornadas no token SAML.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.optionalClaims"
}-->
``` json
{
  "idToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "accessToken": [{"@odata.type": "microsoft.graph.optionalClaim"}],
  "saml2Token": [{"@odata.type": "microsoft.graph.optionalClaim"}]
}
```
