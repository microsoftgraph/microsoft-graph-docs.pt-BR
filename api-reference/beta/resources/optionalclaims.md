---
title: tipo optionalClaims
description: Declara as declarações opcionais solicitadas por um aplicativo.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d6a07685760025cd4aa35429d657a6658dba92b4
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401102"
---
# <a name="optionalclaims-resource-type"></a>tipo de recurso optionalClaims

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Declara as declarações opcionais solicitadas por um aplicativo. Um aplicativo pode configurar declarações opcionais a serem retornadas em cada um dos três tipos de tokens (token de ID, token de acesso, token SAML 2) que pode receber do serviço de token de segurança. Um aplicativo pode configurar um conjunto diferente de declarações opcionais a serem retornadas em cada tipo de token. A propriedade optionalClaims do [aplicativo](application.md) é um objeto **optionalClaims** .

Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações desejam em tokens enviados ao aplicativo pelo serviço de token de segurança da Microsoft. Confira [fornecer declarações opcionais ao aplicativo Azure AD](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|idToken|coleção [optionalClaim](optionalclaim.md)| As declarações opcionais retornadas no token de ID de JWT. |
|accessToken|coleção [optionalClaim](optionalclaim.md)| As declarações opcionais retornadas no token de acesso JWT. |
|saml2Token|coleção [optionalClaim](optionalclaim.md)| As declarações opcionais retornadas no token SAML.|

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