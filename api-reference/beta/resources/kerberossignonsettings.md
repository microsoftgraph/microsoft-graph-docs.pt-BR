---
title: Tipo de recurso kerberosSignOnSettings
description: Representa as configurações kerberos para um aplicativo local publicado por meio do Proxy de Aplicativo.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 0220d6d85c7aafe3489e4099a2c6b1837a7439e2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130084"
---
# <a name="kerberossignonsettings-resource-type"></a>Tipo de recurso kerberosSignOnSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de KCD (Delegação Restrita de Keberos) para o recurso [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) ao publicar um aplicativo local por meio do Proxy de Aplicativo do Azure AD. O Proxy de Aplicativo usa a Delegação Restrita de Kerberos (KCD) para dar suporte ao login único em aplicativos integrados de Autenticação do Windows. Para obter mais informações, consulte Delegação Restrita de Kerberos para fazer o login único em [seus aplicativos com o Proxy de Aplicativo.](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)

>[!NOTE]
>Não use essa propriedade para configurar o SAML ou o single-on baseado em senha. Se você estiver configurando o single-on saml, isso deve ser definido no [servicePrincipal](serviceprincipal.md).
Se você estiver configurando o single-sign baseado em senha, isso deve ser definido usando [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|kerberosServicePrincipalName|String| O SPN de Aplicativo Interno do servidor de aplicativos. Esse SPN precisa estar na lista de serviços para os quais o conector pode apresentar credenciais delegadas. |
|kerberosSignOnMappingAttributeType|String| A Identidade de logon delegada para o conector usar em nome de seus usuários. Para obter mais informações, [consulte Trabalhando com diferentes identidades locais e de nuvem. ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities) Os valores possíveis são: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.kerberosSignOnSettings",
  "baseType": null
}-->

```json
{
  "kerberosServicePrincipalName": "String",
  "kerberosSignOnMappingAttributeType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "kerberosSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
