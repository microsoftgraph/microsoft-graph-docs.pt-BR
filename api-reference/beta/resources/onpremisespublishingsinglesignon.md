---
title: Tipo de recurso kerberosSignOnSettings
description: Representa as configurações de acesso único para um aplicativo local publicado por meio do Proxy de Aplicativo.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 85b2b4963c077b8dcb6ded4818ecc57bce635b39
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134866"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a>Tipo de recurso onPremisesPublishingSingleSignOn

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de login único para o recurso [onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com o Proxy de aplicativo do Azure AD. Esse recurso é usado para definir a Autenticação Integrada do Windows e a autenticação baseada em header como o modo de logo único. Para obter mais informações, consulte Delegação Restrita de Kerberos para fazer o login único em [seus aplicativos com o Proxy de Aplicativo.](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)

>[!NOTE]
>Não use essa propriedade para configurar o SAML ou o single-on baseado em senha. Se você estiver configurando o single-on saml, isso deve ser definido no [servicePrincipal](serviceprincipal.md).
Se você estiver configurando o single-sign baseado em senha, isso deve ser definido usando [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|kerberosSignOnSettings| [kerberosSignOnSettings](kerberossignonsettings.md)| As configurações de Delegação Restrita de Kerberos para aplicativos que usam a Autenticação integrada de janela. |
|singleSignOnMode|String| O modo de login único preferencial para o aplicativo. Os valores possíveis são: `none`, `onPremisesKerberos`, `headerBased`.|

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
