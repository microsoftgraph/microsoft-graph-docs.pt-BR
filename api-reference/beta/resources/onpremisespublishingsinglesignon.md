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
# <a name="onpremisespublishingsinglesignon-resource-type"></a><span data-ttu-id="395df-103">Tipo de recurso onPremisesPublishingSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="395df-103">onPremisesPublishingSingleSignOn resource type</span></span>

<span data-ttu-id="395df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="395df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="395df-105">Representa as configurações de login único para o recurso [onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com o Proxy de aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="395df-105">Represents the single sign-on settings for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Azure AD Application Proxy.</span></span> <span data-ttu-id="395df-106">Esse recurso é usado para definir a Autenticação Integrada do Windows e a autenticação baseada em header como o modo de logo único.</span><span class="sxs-lookup"><span data-stu-id="395df-106">This resource is used for setting Integrated Windows Authentication and header-based authentication as the single-sign on mode.</span></span> <span data-ttu-id="395df-107">Para obter mais informações, consulte Delegação Restrita de Kerberos para fazer o login único em [seus aplicativos com o Proxy de Aplicativo.](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)</span><span class="sxs-lookup"><span data-stu-id="395df-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="395df-108">Não use essa propriedade para configurar o SAML ou o single-on baseado em senha.</span><span class="sxs-lookup"><span data-stu-id="395df-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="395df-109">Se você estiver configurando o single-on saml, isso deve ser definido no [servicePrincipal](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="395df-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="395df-110">Se você estiver configurando o single-sign baseado em senha, isso deve ser definido usando [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span><span class="sxs-lookup"><span data-stu-id="395df-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="395df-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="395df-111">Properties</span></span>

| <span data-ttu-id="395df-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="395df-112">Property</span></span>     | <span data-ttu-id="395df-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="395df-113">Type</span></span>        | <span data-ttu-id="395df-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="395df-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="395df-115">kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="395df-115">kerberosSignOnSettings</span></span>| [<span data-ttu-id="395df-116">kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="395df-116">kerberosSignOnSettings</span></span>](kerberossignonsettings.md)| <span data-ttu-id="395df-117">As configurações de Delegação Restrita de Kerberos para aplicativos que usam a Autenticação integrada de janela.</span><span class="sxs-lookup"><span data-stu-id="395df-117">The Kerberos Constrained Delegation settings for applications that use Integrated Window Authentication.</span></span> |
|<span data-ttu-id="395df-118">singleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="395df-118">singleSignOnMode</span></span>|<span data-ttu-id="395df-119">String</span><span class="sxs-lookup"><span data-stu-id="395df-119">String</span></span>| <span data-ttu-id="395df-120">O modo de login único preferencial para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="395df-120">The preferred single-sign on mode for the application.</span></span> <span data-ttu-id="395df-121">Os valores possíveis são: `none`, `onPremisesKerberos`, `headerBased`.</span><span class="sxs-lookup"><span data-stu-id="395df-121">Possible values are: `none`, `onPremisesKerberos`, `headerBased`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="395df-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="395df-122">JSON representation</span></span>

<span data-ttu-id="395df-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="395df-123">The following is a JSON representation of the resource.</span></span>

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
