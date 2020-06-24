---
title: tipo de recurso kerberosSignOnSettings
description: Representa as configurações Kerberos de um aplicativo local publicado por meio do proxy de aplicativo.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c668380c05c1a76aa971eef85f133a0e9cf8a07
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862535"
---
# <a name="kerberossignonsettings-resource-type"></a>tipo de recurso kerberosSignOnSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de delegação restrita de Keberos (KCD) para o recurso [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) ao publicar um aplicativo local por meio do proxy de aplicativo do Azure AD. O proxy de aplicativo usa a delegação restrita de Kerberos (KCD) para suportar o logon único em aplicativos integrados de autenticação do Windows. Para obter mais informações, consulte [delegação restrita de Kerberos para logon único em seus aplicativos com o proxy de aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).

>[!NOTE]
>Não use essa propriedade para configurar o SAML ou o logon único baseado em senha. Se você estiver configurando o SAML Single-Sign-on, isso deve ser definido no [servicePrincipalName](serviceprincipal.md).
Se você estiver configurando o logon único baseado em senha, ele deverá ser definido usando o [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|kerberosServicePrincipalName|String| O SPN do aplicativo interno do servidor de aplicativos. Esse SPN precisa estar na lista de serviços para os quais o conector pode apresentar credenciais delegadas. |
|kerberosSignOnMappingAttributeType|String| A identidade de logon delegada para o conector usar em nome dos seus usuários. Para obter mais informações, consulte [trabalhando com diferentes identidades locais e de nuvem ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities). Os valores possíveis são: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.|

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