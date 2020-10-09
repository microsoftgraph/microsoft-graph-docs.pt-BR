---
title: tipo de recurso kerberosSignOnSettings
description: Representa as configurações de logon único para um aplicativo local publicado por meio do proxy de aplicativo.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 720690a5e62e39665507b80d3c126b162862b470
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404921"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a>tipo de recurso onPremisesPublishingSingleSignOn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de logon único para o recurso [onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com o proxy de aplicativo do Azure AD. Este recurso é usado para configurar a autenticação integrada do Windows e a autenticação baseada em cabeçalho como o modo de logon único. Para obter mais informações, consulte [delegação restrita de Kerberos para logon único em seus aplicativos com o proxy de aplicativo](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).

>[!NOTE]
>Não use essa propriedade para configurar o SAML ou o logon único baseado em senha. Se você estiver configurando o SAML Single-Sign-on, isso deve ser definido no [servicePrincipalName](serviceprincipal.md).
Se você estiver configurando o logon único baseado em senha, ele deverá ser definido usando o [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|kerberosSignOnSettings| [kerberosSignOnSettings](kerberossignonsettings.md)| As configurações de delegação restritas de Kerberos para aplicativos que usam a autenticação de janela integrada. |
|singleSignOnMode|Cadeia de caracteres| O modo preferencial de logon único para o aplicativo. Os valores possíveis são: `none`, `onPremisesKerberos`, `headerBased`.|

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
  "kerberosSignOnSettings": {"@odata.type": "microsoft.graph.kerberosSignOnSettings"},
  "singleSignOnMode": "String"
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