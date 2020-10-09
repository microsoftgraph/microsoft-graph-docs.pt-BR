---
title: tipo de recurso kerberosSignOnSettings
description: Representa as configurações Kerberos de um aplicativo local publicado por meio do proxy de aplicativo.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 366a220dc8979c55c95706830d4e3d36a920c130
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401143"
---
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="dbaa0-103">tipo de recurso kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="dbaa0-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="dbaa0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbaa0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbaa0-105">Representa as configurações de delegação restrita de Keberos (KCD) para o recurso [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) ao publicar um aplicativo local por meio do proxy de aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dbaa0-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="dbaa0-106">O proxy de aplicativo usa a delegação restrita de Kerberos (KCD) para suportar o logon único em aplicativos integrados de autenticação do Windows.</span><span class="sxs-lookup"><span data-stu-id="dbaa0-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="dbaa0-107">Para obter mais informações, consulte [delegação restrita de Kerberos para logon único em seus aplicativos com o proxy de aplicativo](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span><span class="sxs-lookup"><span data-stu-id="dbaa0-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="dbaa0-108">Não use essa propriedade para configurar o SAML ou o logon único baseado em senha.</span><span class="sxs-lookup"><span data-stu-id="dbaa0-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="dbaa0-109">Se você estiver configurando o SAML Single-Sign-on, isso deve ser definido no [servicePrincipalName](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="dbaa0-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="dbaa0-110">Se você estiver configurando o logon único baseado em senha, ele deverá ser definido usando o [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span><span class="sxs-lookup"><span data-stu-id="dbaa0-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dbaa0-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbaa0-111">Properties</span></span>

| <span data-ttu-id="dbaa0-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbaa0-112">Property</span></span>     | <span data-ttu-id="dbaa0-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbaa0-113">Type</span></span>        | <span data-ttu-id="dbaa0-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbaa0-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dbaa0-115">kerberosServicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="dbaa0-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="dbaa0-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbaa0-116">String</span></span>| <span data-ttu-id="dbaa0-117">O SPN do aplicativo interno do servidor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="dbaa0-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="dbaa0-118">Esse SPN precisa estar na lista de serviços para os quais o conector pode apresentar credenciais delegadas.</span><span class="sxs-lookup"><span data-stu-id="dbaa0-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="dbaa0-119">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="dbaa0-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="dbaa0-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbaa0-120">String</span></span>| <span data-ttu-id="dbaa0-121">A identidade de logon delegada para o conector usar em nome dos seus usuários.</span><span class="sxs-lookup"><span data-stu-id="dbaa0-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="dbaa0-122">Para obter mais informações, consulte [trabalhando com diferentes identidades locais e de nuvem ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span><span class="sxs-lookup"><span data-stu-id="dbaa0-122">For more information, see [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="dbaa0-123">Os valores possíveis são: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span><span class="sxs-lookup"><span data-stu-id="dbaa0-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbaa0-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbaa0-124">JSON representation</span></span>

<span data-ttu-id="dbaa0-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbaa0-125">The following is a JSON representation of the resource.</span></span>

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