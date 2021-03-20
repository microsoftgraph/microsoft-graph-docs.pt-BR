---
title: Tipo de recurso kerberosSignOnSettings
description: Representa as configurações kerberos para um aplicativo local publicado por meio do Proxy de Aplicativo.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: af00e70e1ef4603c1b1370ec5ef9e9ba75fecb4c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943657"
---
# <a name="kerberossignonsettings-resource-type"></a>Tipo de recurso kerberosSignOnSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de Delegação Restrita keberos (KCD) para o recurso [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) ao publicar um aplicativo local por meio do Proxy de Aplicativo do Azure AD. O Proxy de Aplicativo usa o KCD (Delegação Restrita kerberos) para dar suporte a um único login em aplicativos integrados de Autenticação do Windows. Para obter mais informações, [consulte Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).

>[!NOTE]
>Não use essa propriedade para configurar SAML ou acesso único baseado em senha. Se você estiver configurando o SAML single-sign-on, isso deve ser definido no [servicePrincipal](serviceprincipal.md).
Se você estiver configurando um sinal único baseado em senha, isso deve ser definido usando [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|kerberosServicePrincipalName|Cadeia de caracteres| O SPN de Aplicativo Interno do servidor de aplicativos. Esse SPN precisa estar na lista de serviços aos quais o conector pode apresentar credenciais delegadas. |
|kerberosSignOnMappingAttributeType|kerberosSignOnMappingAttributeType| A Identidade de Logon Delegada para o conector a ser usado em nome de seus usuários. Para obter mais informações, consulte [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities). Os valores possíveis são: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.|

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
