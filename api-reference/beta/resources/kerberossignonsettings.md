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
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="1fca4-103">Tipo de recurso kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="1fca4-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="1fca4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fca4-105">Representa as configurações de Delegação Restrita keberos (KCD) para o recurso [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) ao publicar um aplicativo local por meio do Proxy de Aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1fca4-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="1fca4-106">O Proxy de Aplicativo usa o KCD (Delegação Restrita kerberos) para dar suporte a um único login em aplicativos integrados de Autenticação do Windows.</span><span class="sxs-lookup"><span data-stu-id="1fca4-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="1fca4-107">Para obter mais informações, [consulte Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span><span class="sxs-lookup"><span data-stu-id="1fca4-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="1fca4-108">Não use essa propriedade para configurar SAML ou acesso único baseado em senha.</span><span class="sxs-lookup"><span data-stu-id="1fca4-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="1fca4-109">Se você estiver configurando o SAML single-sign-on, isso deve ser definido no [servicePrincipal](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="1fca4-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="1fca4-110">Se você estiver configurando um sinal único baseado em senha, isso deve ser definido usando [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span><span class="sxs-lookup"><span data-stu-id="1fca4-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1fca4-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fca4-111">Properties</span></span>

| <span data-ttu-id="1fca4-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fca4-112">Property</span></span>     | <span data-ttu-id="1fca4-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fca4-113">Type</span></span>        | <span data-ttu-id="1fca4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fca4-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1fca4-115">kerberosServicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="1fca4-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="1fca4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fca4-116">String</span></span>| <span data-ttu-id="1fca4-117">O SPN de Aplicativo Interno do servidor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1fca4-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="1fca4-118">Esse SPN precisa estar na lista de serviços aos quais o conector pode apresentar credenciais delegadas.</span><span class="sxs-lookup"><span data-stu-id="1fca4-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="1fca4-119">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="1fca4-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="1fca4-120">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="1fca4-120">kerberosSignOnMappingAttributeType</span></span>| <span data-ttu-id="1fca4-121">A Identidade de Logon Delegada para o conector a ser usado em nome de seus usuários.</span><span class="sxs-lookup"><span data-stu-id="1fca4-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="1fca4-122">Para obter mais informações, consulte [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span><span class="sxs-lookup"><span data-stu-id="1fca4-122">For more information, see [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="1fca4-123">Os valores possíveis são: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span><span class="sxs-lookup"><span data-stu-id="1fca4-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fca4-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fca4-124">JSON representation</span></span>

<span data-ttu-id="1fca4-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fca4-125">The following is a JSON representation of the resource.</span></span>

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
