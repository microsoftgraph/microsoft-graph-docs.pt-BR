---
title: Tipo de recurso appleManagedIdentityProvider
description: Representa o provedor de identidade apple em um locatário do B2C do Azure AD
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: ee02900b6d41695d49d7c5ee38d834c676f69603
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491065"
---
# <a name="applemanagedidentityprovider-resource-type"></a><span data-ttu-id="fd532-103">Tipo de recurso appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="fd532-103">appleManagedIdentityProvider resource type</span></span>
<span data-ttu-id="fd532-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd532-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd532-105">Você pode configurar a Apple como um provedor de identidade social para um locatário do B2C do Azure AD</span><span class="sxs-lookup"><span data-stu-id="fd532-105">You can configure Apple as a social identity provider for an Azure AD B2C tenant.</span></span> <span data-ttu-id="fd532-106">Com base nas informações fornecidas pela Apple, a API irá gerar um segredo do cliente.</span><span class="sxs-lookup"><span data-stu-id="fd532-106">Based on the information Apple provides, the API will generate a client secret.</span></span> <span data-ttu-id="fd532-107">A Apple precisa que o segredo seja renovado a cada seis meses.</span><span class="sxs-lookup"><span data-stu-id="fd532-107">Apple needs the secret to be renewed every six months.</span></span> <span data-ttu-id="fd532-108">Você terá que girar o segredo manualmente.</span><span class="sxs-lookup"><span data-stu-id="fd532-108">You will have to maunally rotate the secret.</span></span>

<span data-ttu-id="fd532-109">Este tipo herdará de [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="fd532-109">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fd532-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="fd532-110">Methods</span></span>

| <span data-ttu-id="fd532-111">Método</span><span class="sxs-lookup"><span data-stu-id="fd532-111">Method</span></span>       | <span data-ttu-id="fd532-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fd532-112">Return Type</span></span>  |<span data-ttu-id="fd532-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd532-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fd532-114">List</span><span class="sxs-lookup"><span data-stu-id="fd532-114">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="fd532-115">Coleção identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="fd532-115">identityProviderBase collection</span></span>|<span data-ttu-id="fd532-116">Recupere todos os provedores de identidade configurados em um locatário, incluindo os provedores de identidade Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-116">Retrieve all identity providers configured in a tenant including the Apple identity providers.</span></span>|
|[<span data-ttu-id="fd532-117">Create</span><span class="sxs-lookup"><span data-stu-id="fd532-117">Create</span></span>](../api/identityproviderbase-post-identityproviders.md)|<span data-ttu-id="fd532-118">appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="fd532-118">appleManagedIdentityProvider</span></span> |<span data-ttu-id="fd532-119">Criae uma nova configuração de provedor de identidade Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-119">Create a new Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="fd532-120">Get</span><span class="sxs-lookup"><span data-stu-id="fd532-120">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="fd532-121">appleManagedIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="fd532-121">appleManagedIdentityProvider</span></span> |<span data-ttu-id="fd532-122">Recuperar propriedades da configuração do provedor de identidade Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-122">Retrieve properties of the Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="fd532-123">Atualizar</span><span class="sxs-lookup"><span data-stu-id="fd532-123">Update</span></span>](../api/identityproviderbase-update.md)|<span data-ttu-id="fd532-124">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="fd532-124">None</span></span>|<span data-ttu-id="fd532-125">Atualizar a configuração do provedor de identidade Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-125">Update the Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="fd532-126">Delete</span><span class="sxs-lookup"><span data-stu-id="fd532-126">Delete</span></span>](../api/identityproviderbase-delete.md)|<span data-ttu-id="fd532-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd532-127">None</span></span>|<span data-ttu-id="fd532-128">Excluir a configuração do provedor de identidade Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-128">Delete the Apple identity provider configuration.</span></span>|
|[<span data-ttu-id="fd532-129">Listar os tipos de provedor disponíveis</span><span class="sxs-lookup"><span data-stu-id="fd532-129">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="fd532-130">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd532-130">String collection</span></span>|<span data-ttu-id="fd532-131">Recuperar todos os tipos de provedor de identidade disponíveis no locatário.</span><span class="sxs-lookup"><span data-stu-id="fd532-131">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd532-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd532-132">Properties</span></span>

|<span data-ttu-id="fd532-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd532-133">Property</span></span>|<span data-ttu-id="fd532-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd532-134">Type</span></span>|<span data-ttu-id="fd532-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd532-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd532-136">developerId</span><span class="sxs-lookup"><span data-stu-id="fd532-136">developerId</span></span>|<span data-ttu-id="fd532-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd532-137">String</span></span>|<span data-ttu-id="fd532-138">O Identificador de desenvolvedor da Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-138">The Apple developer identifier.</span></span> <span data-ttu-id="fd532-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd532-139">Required.</span></span>|
|<span data-ttu-id="fd532-140">serviceId</span><span class="sxs-lookup"><span data-stu-id="fd532-140">serviceId</span></span>|<span data-ttu-id="fd532-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd532-141">String</span></span>|<span data-ttu-id="fd532-142">O identificador de serviço da Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-142">The Apple service identifier.</span></span> <span data-ttu-id="fd532-143">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd532-143">Required.</span></span>|
|<span data-ttu-id="fd532-144">keyId</span><span class="sxs-lookup"><span data-stu-id="fd532-144">keyId</span></span>|<span data-ttu-id="fd532-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd532-145">String</span></span>|<span data-ttu-id="fd532-146">O identificador de chave da Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-146">The Apple key identifier.</span></span> <span data-ttu-id="fd532-147">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd532-147">Required.</span></span>|
|<span data-ttu-id="fd532-148">certificateData</span><span class="sxs-lookup"><span data-stu-id="fd532-148">certificateData</span></span>|<span data-ttu-id="fd532-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd532-149">String</span></span>|<span data-ttu-id="fd532-150">Os dados do certificado, que são uma longa sequência de texto do certificado, podem ser nulos.</span><span class="sxs-lookup"><span data-stu-id="fd532-150">The certificate data which is a long string of text from the certificate, can be null.</span></span>|
|<span data-ttu-id="fd532-151">id</span><span class="sxs-lookup"><span data-stu-id="fd532-151">id</span></span>|<span data-ttu-id="fd532-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd532-152">String</span></span>|<span data-ttu-id="fd532-153">O identificador do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fd532-153">The identifier of the identity provider.</span></span> <span data-ttu-id="fd532-154">Herdado de [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="fd532-154">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="fd532-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd532-155">Read-only.</span></span>|
|<span data-ttu-id="fd532-156">displayName</span><span class="sxs-lookup"><span data-stu-id="fd532-156">displayName</span></span>|<span data-ttu-id="fd532-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd532-157">String</span></span>|<span data-ttu-id="fd532-158">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="fd532-158">The display name of the identity provider.</span></span> <span data-ttu-id="fd532-159">Herdado de [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="fd532-159">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|

<span data-ttu-id="fd532-160">Você pode encontrar o developerId, serviceId, keyId e o certificateData no portal do desenvolvedor da Apple.</span><span class="sxs-lookup"><span data-stu-id="fd532-160">You can find the developerId, serviceId, keyId and the certificateData from the Apple developer portal.</span></span> <span data-ttu-id="fd532-161">Para obter mais detalhes, você pode seguir o guia para [criar um aplicativo Apple ID](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)</span><span class="sxs-lookup"><span data-stu-id="fd532-161">For nore details you can follow the guide to [create an Apple ID application](/azure/active-directory-b2c/identity-provider-apple-id?pivots=b2c-user-flow#create-an-apple-id-application)</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd532-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd532-162">JSON representation</span></span>

<span data-ttu-id="fd532-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd532-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```json
{
    "id": "String",
    "displayName": "String",
    "developerId": "String",
    "serviceId": "String",
    "keyId": "String",
    "certificateData": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "appleIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
