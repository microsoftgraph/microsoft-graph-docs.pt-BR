---
title: tipo de recurso kerberosSignOnSettings
description: Representa as configurações de logon único para um aplicativo local publicado por meio do proxy de aplicativo.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f07fc81fee6fdc8e8ff3b55c246facdc4f155d11
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556376"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a>tipo de recurso onPremisesPublishingSingleSignOn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de logon único para o recurso [onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com o proxy de aplicativo do Azure AD. Este recurso é usado para configurar a autenticação integrada do Windows e a autenticação baseada em cabeçalho como o modo de logon único. Para obter mais informações, consulte [delegação restrita de Kerberos para logon único em seus aplicativos com o proxy de aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).

>[!NOTE]
>Não use essa propriedade para configurar o SAML ou o logon único baseado em senha. Se você estiver configurando o SAML Single-Sign-on, isso deve ser definido no [servicePrincipalName](serviceprincipal.md).
Se você estiver configurando o logon único baseado em senha, ele deverá ser definido usando o [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|kerberosSignOnSettings| [kerberosSignOnSettings](kerberossignonsettings.md)| As configurações de delegação restrita de Kerberos para o aplicativo. |
|singleSignOnMode|String| O modo preferencial de logon único para o aplicativo. Os valores possíveis são: `none`, `onPremisesKerberos`, `headerBased`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishingSingleSignOn",
  "baseType": null
}-->

```json
{
  "KerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "SingleSignOnMode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishingSingleSignOn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->