---
title: tipo de recurso socialIdentityProvider
description: Representa provedores de identidade social em um locatário do Azure Active Directory e um locatário do Azure AD B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 58e08852c99c97648447e7d0acf9946ea3227122
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491055"
---
# <a name="socialidentityprovider-resource-type"></a><span data-ttu-id="1be8f-103">tipo de recurso socialIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="1be8f-103">socialIdentityProvider resource type</span></span>
<span data-ttu-id="1be8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1be8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1be8f-105">Representa provedores de identidade social com [Identidades Externas](/azure/active-directory/external-identities/) tanto para locatário do Azure Active Directory quanto para um locatário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="1be8f-105">Represents social identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="1be8f-106">Este tipo herdará de [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="1be8f-106">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

<span data-ttu-id="1be8f-107">Para cenários do Azure AD B2B em um locatário do Microsoft Azure Active Directory, o tipo de provedor de identidade pode ser o Google ou o Facebook.</span><span class="sxs-lookup"><span data-stu-id="1be8f-107">For Azure AD B2B scenarios in an Azure AD tenant, the identity provider type can be Google or Facebook.</span></span>

<span data-ttu-id="1be8f-108">A configuração de um provedor de identidade no locatário do Microsoft Azure Active Directory permite novos cenários de convidado no Azure AD B2B.</span><span class="sxs-lookup"><span data-stu-id="1be8f-108">Configuring an identity provider in your Azure AD tenant enables new Azure AD B2B guest scenarios.</span></span> <span data-ttu-id="1be8f-109">Por exemplo, uma organização possui recursos no Microsoft 365 que precisam ser compartilhados com um usuário do Gmail.</span><span class="sxs-lookup"><span data-stu-id="1be8f-109">For example, an organization has resources in Microsoft 365 that need to be shared with a Gmail user.</span></span> <span data-ttu-id="1be8f-110">O usuário do Gmail usará as credenciais de conta do Google para autenticar e acessar os documentos.</span><span class="sxs-lookup"><span data-stu-id="1be8f-110">The Gmail user will use their Google account credentials to authenticate and access the documents.</span></span>

<span data-ttu-id="1be8f-111">Em um locatário do Azure AD B2C, o tipo de provedor de identidade pode ser Microsoft, Google, Facebook, Amazon, LinkedIn ou Twitter.</span><span class="sxs-lookup"><span data-stu-id="1be8f-111">In an Azure AD B2C tenant, the identity provider type can be Microsoft, Google, Facebook, Amazon, LinkedIn or Twitter.</span></span> <span data-ttu-id="1be8f-112">Os seguintes provedores de identidade estão em visualização: Weibo, QQ, WeChat e GitHub.</span><span class="sxs-lookup"><span data-stu-id="1be8f-112">The following identity providers are in preview: Weibo, QQ, WeChat, and GitHub.</span></span>

<span data-ttu-id="1be8f-113">Configurar um provedor de identidade em seu locatário do Azure AD B2C permite que os usuários se inscrevam e entrem usando um provedor com suporte de conta social em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1be8f-113">Configuring an identity provider in your Azure AD B2C tenant enables users to sign up and sign in using a social account supported provider in an application.</span></span> <span data-ttu-id="1be8f-114">Por exemplo, um aplicativo pode usar o Azure AD B2C para permitir que os usuários se inscrevam no serviço usando uma conta do Facebook.</span><span class="sxs-lookup"><span data-stu-id="1be8f-114">For example, an application can use Azure AD B2C to allow users to sign up for the service using a Facebook account.</span></span>

## <a name="methods"></a><span data-ttu-id="1be8f-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="1be8f-115">Methods</span></span>

| <span data-ttu-id="1be8f-116">Método</span><span class="sxs-lookup"><span data-stu-id="1be8f-116">Method</span></span>       | <span data-ttu-id="1be8f-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1be8f-117">Return Type</span></span>  |<span data-ttu-id="1be8f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1be8f-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1be8f-119">List</span><span class="sxs-lookup"><span data-stu-id="1be8f-119">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="1be8f-120">Coleção [identityProviderBase](../resources/identityproviderbase.md)</span><span class="sxs-lookup"><span data-stu-id="1be8f-120">[identityProviderBase](../resources/identityproviderbase.md) collection</span></span>|<span data-ttu-id="1be8f-121">Recuperar todos os provedores de identidade configurados em um locatário, incluindo os provedores de identidade social.</span><span class="sxs-lookup"><span data-stu-id="1be8f-121">Retrieve all identity providers configured in a tenant including the social identity providers.</span></span>|
|[<span data-ttu-id="1be8f-122">Criar</span><span class="sxs-lookup"><span data-stu-id="1be8f-122">Create</span></span>](../api/identityproviderbase-post-identityproviders.md)|<span data-ttu-id="1be8f-123">socialidentityprovider</span><span class="sxs-lookup"><span data-stu-id="1be8f-123">socialidentityprovider</span></span> |<span data-ttu-id="1be8f-124">Criar um novo provedor de identidade social.</span><span class="sxs-lookup"><span data-stu-id="1be8f-124">Create a new social identity provider.</span></span>|
|[<span data-ttu-id="1be8f-125">Obter</span><span class="sxs-lookup"><span data-stu-id="1be8f-125">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="1be8f-126">socialidentityprovider</span><span class="sxs-lookup"><span data-stu-id="1be8f-126">socialidentityprovider</span></span> |<span data-ttu-id="1be8f-127">Recuperar propriedades de um provedor de identidade social.</span><span class="sxs-lookup"><span data-stu-id="1be8f-127">Retrieve properties of a social identity provider.</span></span>|
|[<span data-ttu-id="1be8f-128">Atualizar</span><span class="sxs-lookup"><span data-stu-id="1be8f-128">Update</span></span>](../api/identityproviderbase-update.md)|<span data-ttu-id="1be8f-129">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="1be8f-129">None</span></span>|<span data-ttu-id="1be8f-130">Atualizar um provedor de identidade social.</span><span class="sxs-lookup"><span data-stu-id="1be8f-130">Update a social identity provider.</span></span>|
|[<span data-ttu-id="1be8f-131">Delete</span><span class="sxs-lookup"><span data-stu-id="1be8f-131">Delete</span></span>](../api/identityproviderbase-delete.md)|<span data-ttu-id="1be8f-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1be8f-132">None</span></span>|<span data-ttu-id="1be8f-133">Excluir um provedor de  identidade social.</span><span class="sxs-lookup"><span data-stu-id="1be8f-133">Delete a social  identity provider.</span></span>|
|[<span data-ttu-id="1be8f-134">Listar os tipos de provedor disponíveis</span><span class="sxs-lookup"><span data-stu-id="1be8f-134">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="1be8f-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1be8f-135">String collection</span></span>|<span data-ttu-id="1be8f-136">Recuperar todos os tipos de provedores de identidade disponíveis no locatário.</span><span class="sxs-lookup"><span data-stu-id="1be8f-136">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="1be8f-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1be8f-137">Properties</span></span>

|<span data-ttu-id="1be8f-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1be8f-138">Property</span></span>|<span data-ttu-id="1be8f-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="1be8f-139">Type</span></span>|<span data-ttu-id="1be8f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="1be8f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1be8f-141">clientId</span><span class="sxs-lookup"><span data-stu-id="1be8f-141">clientId</span></span>|<span data-ttu-id="1be8f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1be8f-142">String</span></span>|<span data-ttu-id="1be8f-143">O identificador do cliente para o aplicativo obtido ao registrar o aplicativo com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1be8f-143">The client identifier for the application obtained when registering the application with the identity provider.</span></span> <span data-ttu-id="1be8f-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1be8f-144">Required.</span></span>|
|<span data-ttu-id="1be8f-145">clientSecret</span><span class="sxs-lookup"><span data-stu-id="1be8f-145">clientSecret</span></span>|<span data-ttu-id="1be8f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1be8f-146">String</span></span>|<span data-ttu-id="1be8f-147">O segredo do cliente para o aplicativo obtido quando o aplicativo é registrado com o provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1be8f-147">The client secret for the application that is obtained when the application is registered with the identity provider.</span></span> <span data-ttu-id="1be8f-148">Isso é somente gravação.</span><span class="sxs-lookup"><span data-stu-id="1be8f-148">This is write-only.</span></span> <span data-ttu-id="1be8f-149">Uma operação de leitura retorna "\*\*\*\*".</span><span class="sxs-lookup"><span data-stu-id="1be8f-149">A read operation returns "\*\*\*\*".</span></span> <span data-ttu-id="1be8f-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1be8f-150">Required.</span></span>|
|<span data-ttu-id="1be8f-151">id</span><span class="sxs-lookup"><span data-stu-id="1be8f-151">id</span></span>|<span data-ttu-id="1be8f-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1be8f-152">String</span></span>|<span data-ttu-id="1be8f-153">O identificador do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1be8f-153">The identifier of the identity provider.</span></span> <span data-ttu-id="1be8f-154">Herdado de [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="1be8f-154">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="1be8f-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1be8f-155">Read-only.</span></span>|
|<span data-ttu-id="1be8f-156">displayName</span><span class="sxs-lookup"><span data-stu-id="1be8f-156">displayName</span></span>|<span data-ttu-id="1be8f-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1be8f-157">String</span></span>|<span data-ttu-id="1be8f-158">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1be8f-158">The display name of the identity provider.</span></span> <span data-ttu-id="1be8f-159">Herdado de [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="1be8f-159">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|
|<span data-ttu-id="1be8f-160">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="1be8f-160">identityProviderType</span></span>|<span data-ttu-id="1be8f-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1be8f-161">String</span></span>|<span data-ttu-id="1be8f-162">Para um cenário B2B, valores possíveis: `Google`, `Facebook`.</span><span class="sxs-lookup"><span data-stu-id="1be8f-162">For a B2B scenario, possible values: `Google`, `Facebook`.</span></span> <span data-ttu-id="1be8f-163">Para um cenário B2C, valores possíveis: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span><span class="sxs-lookup"><span data-stu-id="1be8f-163">For a B2C scenario, possible values: `Microsoft`, `Google`, `Amazon`, `LinkedIn`, `Facebook`, `GitHub`, `Twitter`, `Weibo`, `QQ`, `WeChat`.</span></span> <span data-ttu-id="1be8f-164">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1be8f-164">Required.</span></span>|

### <a name="where-to-get-the-client-identifier-and-secret"></a><span data-ttu-id="1be8f-165">Onde obter o identificador e o segredo do cliente</span><span class="sxs-lookup"><span data-stu-id="1be8f-165">Where to get the client identifier and secret</span></span>

<span data-ttu-id="1be8f-166">Cada provedor de identidade tem um processo para criar um registro do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1be8f-166">Each identity provider has a process for creating an app registration.</span></span> <span data-ttu-id="1be8f-167">Por exemplo, os usuários criam um registro de aplicativo com o Facebook no [developers.facebook.com](https://developers.facebook.com/).</span><span class="sxs-lookup"><span data-stu-id="1be8f-167">For example, users create an app registration with Facebook at [developers.facebook.com](https://developers.facebook.com/).</span></span> <span data-ttu-id="1be8f-168">O identificador do cliente e o segredo do cliente resultantes podem ser passados para [criar identityProvider](../api/identityproviderbase-post-identityproviders.md).</span><span class="sxs-lookup"><span data-stu-id="1be8f-168">The resulting client identifier and client secret can be passed to [create identityProvider](../api/identityproviderbase-post-identityproviders.md).</span></span> <span data-ttu-id="1be8f-169">Em seguida, cada objeto de usuário no diretório pode ser federado para qualquer um dos provedores de identidade do locatário para autenticação.</span><span class="sxs-lookup"><span data-stu-id="1be8f-169">Then, each user object in the directory can be federated to any of the tenant's identity providers for authentication.</span></span> <span data-ttu-id="1be8f-170">Isso permite que o usuário entre inserindo credenciais na página de entrada do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1be8f-170">This enables the user to sign in by entering credentials on the identity provider's sign-in page.</span></span> <span data-ttu-id="1be8f-171">O token do provedor de identidade é validado pelo Azure AD antes que o locatário emita um token ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1be8f-171">The token from the identity provider is validated by Azure AD before the tenant issues a token to the application.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1be8f-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1be8f-172">JSON representation</span></span>

<span data-ttu-id="1be8f-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1be8f-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "socialIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
