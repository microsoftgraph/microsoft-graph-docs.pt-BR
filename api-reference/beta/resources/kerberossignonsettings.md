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
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="b1867-103">Tipo de recurso kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="b1867-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="b1867-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1867-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1867-105">Representa as configurações de KCD (Delegação Restrita de Keberos) para o recurso [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) ao publicar um aplicativo local por meio do Proxy de Aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1867-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="b1867-106">O Proxy de Aplicativo usa a Delegação Restrita de Kerberos (KCD) para dar suporte ao login único em aplicativos integrados de Autenticação do Windows.</span><span class="sxs-lookup"><span data-stu-id="b1867-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="b1867-107">Para obter mais informações, consulte Delegação Restrita de Kerberos para fazer o login único em [seus aplicativos com o Proxy de Aplicativo.](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)</span><span class="sxs-lookup"><span data-stu-id="b1867-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="b1867-108">Não use essa propriedade para configurar o SAML ou o single-on baseado em senha.</span><span class="sxs-lookup"><span data-stu-id="b1867-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="b1867-109">Se você estiver configurando o single-on saml, isso deve ser definido no [servicePrincipal](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="b1867-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="b1867-110">Se você estiver configurando o single-sign baseado em senha, isso deve ser definido usando [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span><span class="sxs-lookup"><span data-stu-id="b1867-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b1867-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1867-111">Properties</span></span>

| <span data-ttu-id="b1867-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1867-112">Property</span></span>     | <span data-ttu-id="b1867-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1867-113">Type</span></span>        | <span data-ttu-id="b1867-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1867-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1867-115">kerberosServicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1867-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="b1867-116">String</span><span class="sxs-lookup"><span data-stu-id="b1867-116">String</span></span>| <span data-ttu-id="b1867-117">O SPN de Aplicativo Interno do servidor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b1867-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="b1867-118">Esse SPN precisa estar na lista de serviços para os quais o conector pode apresentar credenciais delegadas.</span><span class="sxs-lookup"><span data-stu-id="b1867-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="b1867-119">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="b1867-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="b1867-120">String</span><span class="sxs-lookup"><span data-stu-id="b1867-120">String</span></span>| <span data-ttu-id="b1867-121">A Identidade de logon delegada para o conector usar em nome de seus usuários.</span><span class="sxs-lookup"><span data-stu-id="b1867-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="b1867-122">Para obter mais informações, [consulte Trabalhando com diferentes identidades locais e de nuvem. ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities)</span><span class="sxs-lookup"><span data-stu-id="b1867-122">For more information, see [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="b1867-123">Os valores possíveis são: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span><span class="sxs-lookup"><span data-stu-id="b1867-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1867-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1867-124">JSON representation</span></span>

<span data-ttu-id="b1867-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1867-125">The following is a JSON representation of the resource.</span></span>

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
