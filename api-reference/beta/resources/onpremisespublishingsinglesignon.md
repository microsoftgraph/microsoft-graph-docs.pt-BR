---
title: tipo de recurso kerberosSignOnSettings
description: Representa as configurações de logon único para um aplicativo local publicado por meio do proxy de aplicativo.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ebe5c584b009bd3028aece3cbfca75463f9c86dd
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862455"
---
# <a name="onpremisespublishingsinglesignon-resource-type"></a><span data-ttu-id="f7259-103">tipo de recurso onPremisesPublishingSingleSignOn</span><span class="sxs-lookup"><span data-stu-id="f7259-103">onPremisesPublishingSingleSignOn resource type</span></span>

<span data-ttu-id="f7259-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7259-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7259-105">Representa as configurações de logon único para o recurso [onPremisesPublishing](onpremisespublishing.md) ao publicar um aplicativo local com o proxy de aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f7259-105">Represents the single sign-on settings for the [onPremisesPublishing](onpremisespublishing.md) resource when publishing an on-premises application with Azure AD Application Proxy.</span></span> <span data-ttu-id="f7259-106">Este recurso é usado para configurar a autenticação integrada do Windows e a autenticação baseada em cabeçalho como o modo de logon único.</span><span class="sxs-lookup"><span data-stu-id="f7259-106">This resource is used for setting Integrated Windows Authentication and header-based authentication as the single-sign on mode.</span></span> <span data-ttu-id="f7259-107">Para obter mais informações, consulte [delegação restrita de Kerberos para logon único em seus aplicativos com o proxy de aplicativo](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span><span class="sxs-lookup"><span data-stu-id="f7259-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="f7259-108">Não use essa propriedade para configurar o SAML ou o logon único baseado em senha.</span><span class="sxs-lookup"><span data-stu-id="f7259-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="f7259-109">Se você estiver configurando o SAML Single-Sign-on, isso deve ser definido no [servicePrincipalName](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="f7259-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="f7259-110">Se você estiver configurando o logon único baseado em senha, ele deverá ser definido usando o [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span><span class="sxs-lookup"><span data-stu-id="f7259-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f7259-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7259-111">Properties</span></span>

| <span data-ttu-id="f7259-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7259-112">Property</span></span>     | <span data-ttu-id="f7259-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7259-113">Type</span></span>        | <span data-ttu-id="f7259-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7259-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7259-115">kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="f7259-115">kerberosSignOnSettings</span></span>| [<span data-ttu-id="f7259-116">kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="f7259-116">kerberosSignOnSettings</span></span>](kerberossignonsettings.md)| <span data-ttu-id="f7259-117">As configurações de delegação restritas de Kerberos para aplicativos que usam a autenticação de janela integrada.</span><span class="sxs-lookup"><span data-stu-id="f7259-117">The Kerberos Constrained Delegation settings for applications that use Integrated Window Authentication.</span></span> |
|<span data-ttu-id="f7259-118">singleSignOnMode</span><span class="sxs-lookup"><span data-stu-id="f7259-118">singleSignOnMode</span></span>|<span data-ttu-id="f7259-119">String</span><span class="sxs-lookup"><span data-stu-id="f7259-119">String</span></span>| <span data-ttu-id="f7259-120">O modo preferencial de logon único para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f7259-120">The preferred single-sign on mode for the application.</span></span> <span data-ttu-id="f7259-121">Os valores possíveis são: `none`, `onPremisesKerberos`, `headerBased`.</span><span class="sxs-lookup"><span data-stu-id="f7259-121">Possible values are: `none`, `onPremisesKerberos`, `headerBased`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7259-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7259-122">JSON representation</span></span>

<span data-ttu-id="f7259-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7259-123">The following is a JSON representation of the resource.</span></span>

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