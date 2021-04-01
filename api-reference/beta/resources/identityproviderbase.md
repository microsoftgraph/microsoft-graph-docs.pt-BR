---
title: Tipo de recurso identityProviderBase
description: Representa provedores de identidade em um locatário do Azure Active Directory e um locatário do B2C do Azure AD
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 1a3d26697c26b803bcbac9141d7ff011575f91f7
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491072"
---
# <a name="identityproviderbase-resource-type"></a><span data-ttu-id="b0ab8-103">Tipo de recurso identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="b0ab8-103">identityProviderBase resource type</span></span>
<span data-ttu-id="b0ab8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0ab8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0ab8-105">Representa provedores de identidade com [Identidades externas](/azure/active-directory/external-identities/) para locatário do Azure Active Directory e um locatário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-105">Represents identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="b0ab8-106">Para cenários do Azure AD B2B em um diretório do Azure AD, o provedor de identidade pode ser um [provedor de identidade social](../resources/socialidentityprovider.md) ou um [provedor de identidade interno](../resources/builtinidentityprovider.md), que herdará do tipo de recurso base do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-106">For Azure AD B2B scenarios in an Azure AD directory, the identity provider can be a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md), which will inherit from identityProviderBase resource type.</span></span>

<span data-ttu-id="b0ab8-107">Configurar um provedor de identidade em seu diretório do Azure AD permite novos cenários de convidado do Azure AD B2B.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-107">Configuring an identity provider in your Azure AD directory enables new Azure AD B2B guest scenarios.</span></span> <span data-ttu-id="b0ab8-108">Por exemplo, uma organização possui recursos no Microsoft 365 que precisam ser compartilhados com um usuário do Gmail.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-108">For example, an organization has resources in Microsoft 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="b0ab8-109">O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-109">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

<span data-ttu-id="b0ab8-110">Em um diretório Azure AD B2C, o tipo de provedor de identidade podem ser [Provedores de identidade social](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [appleIdentityProvider](../resources/appleidentityprovider.md), que herdará do tipo de recurso identityProviderBase. </span><span class="sxs-lookup"><span data-stu-id="b0ab8-110">In an Azure AD B2C directory, the identity provider type can be a [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or [appleIdentityProvider](../resources/appleidentityprovider.md), which will inherit from identityProviderBase resource type.</span></span>

<span data-ttu-id="b0ab8-111">Configurar um provedor de identidade no diretório do Azure AD B2C permite que os usuários se inscrevam e entrem usando uma conta social ou um provedor com suporte OpenID Connect personalizado em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-111">Configuring an identity provider in your Azure AD B2C directory enables users to sign up and sign in using a social account or a custom OpenID Connect supported provider in an application.</span></span> <span data-ttu-id="b0ab8-112">Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook ou o seu próprio provedor de identidade personalizado que esteja em conformidade com o protocolo OIDC.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-112">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account or their own custom identity provider that complies with OIDC protocol.</span></span>

## <a name="methods"></a><span data-ttu-id="b0ab8-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0ab8-113">Methods</span></span>

| <span data-ttu-id="b0ab8-114">Método</span><span class="sxs-lookup"><span data-stu-id="b0ab8-114">Method</span></span>       | <span data-ttu-id="b0ab8-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0ab8-115">Return Type</span></span>  |<span data-ttu-id="b0ab8-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ab8-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0ab8-117">List</span><span class="sxs-lookup"><span data-stu-id="b0ab8-117">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="b0ab8-118">Coleção identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="b0ab8-118">identityProviderBase collection</span></span>|<span data-ttu-id="b0ab8-119">Recupere todos os provedores de identidade configurados em um locatário.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-119">Retrieve all identity providers configured in a tenant.</span></span>|
|[<span data-ttu-id="b0ab8-120">Listar os tipos de provedor disponíveis</span><span class="sxs-lookup"><span data-stu-id="b0ab8-120">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="b0ab8-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0ab8-121">String collection</span></span>|<span data-ttu-id="b0ab8-122">Recupere todos os tipos de provedor de identidade disponíveis no locatário.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-122">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0ab8-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0ab8-123">Properties</span></span>

|<span data-ttu-id="b0ab8-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0ab8-124">Property</span></span>|<span data-ttu-id="b0ab8-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0ab8-125">Type</span></span>|<span data-ttu-id="b0ab8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0ab8-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0ab8-127">id</span><span class="sxs-lookup"><span data-stu-id="b0ab8-127">id</span></span>|<span data-ttu-id="b0ab8-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0ab8-128">String</span></span>|<span data-ttu-id="b0ab8-129">O identificador do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-129">The identifier of the identity provider.</span></span>|
|<span data-ttu-id="b0ab8-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b0ab8-130">displayName</span></span>|<span data-ttu-id="b0ab8-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0ab8-131">String</span></span>|<span data-ttu-id="b0ab8-132">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-132">The display name of the identity provider.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0ab8-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0ab8-133">JSON representation</span></span>

<span data-ttu-id="b0ab8-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0ab8-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String",
}
```
