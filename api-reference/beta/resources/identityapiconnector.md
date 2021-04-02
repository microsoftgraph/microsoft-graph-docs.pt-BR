---
title: Tipo de recurso identityApiConnector
description: Representa conectores de API em um locatário do Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7ecb96a9ca2f4397c1f0ee52908a7802374df0f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508074"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="e5577-103">Tipo de recurso identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="e5577-103">identityApiConnector resource type</span></span>

<span data-ttu-id="e5577-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5577-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5577-105">Representa conectores de API em um Azure Active Directory (Azure AD) e locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="e5577-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="e5577-106">Um conector de API usado na sua assinatura de autoatendados de Identidades Externas do Azure AD e fluxos de usuário de entrada do Azure AD B2C permite que você chame uma API durante a execução do fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="e5577-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="e5577-107">Um conector de API fornece as informações necessárias para chamar uma API, incluindo uma URL de ponto de extremidade e autenticação.</span><span class="sxs-lookup"><span data-stu-id="e5577-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="e5577-108">Um conector de API pode ser usado em uma etapa específica em um fluxo de usuário para afetar a execução do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="e5577-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="e5577-109">Por exemplo, a resposta da API pode impedir que um usuário se inscreve, mostrar um erro de validação de entrada ou substituir atributos coletados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="e5577-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="e5577-110">Use a [API b2xIdentityUserFlow](b2xidentityuserflow.md) para usar um conector de API de um fluxo de usuário de autoatendência de Identidades Externas.</span><span class="sxs-lookup"><span data-stu-id="e5577-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="e5577-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="e5577-111">Methods</span></span>

|<span data-ttu-id="e5577-112">Método</span><span class="sxs-lookup"><span data-stu-id="e5577-112">Method</span></span>|<span data-ttu-id="e5577-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e5577-113">Return type</span></span>|<span data-ttu-id="e5577-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5577-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5577-115">List</span><span class="sxs-lookup"><span data-stu-id="e5577-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="e5577-116">[Coleção identityApiConnector](identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="e5577-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="e5577-117">Obter uma lista de conectores de API</span><span class="sxs-lookup"><span data-stu-id="e5577-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="e5577-118">Criar</span><span class="sxs-lookup"><span data-stu-id="e5577-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="e5577-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="e5577-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="e5577-120">Crie um novo conector de API.</span><span class="sxs-lookup"><span data-stu-id="e5577-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="e5577-121">Obter</span><span class="sxs-lookup"><span data-stu-id="e5577-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="e5577-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="e5577-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="e5577-123">Leia as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="e5577-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="e5577-124">Atualizar</span><span class="sxs-lookup"><span data-stu-id="e5577-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="e5577-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="e5577-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="e5577-126">Atualize as propriedades de um conector de API.</span><span class="sxs-lookup"><span data-stu-id="e5577-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="e5577-127">Carregar certificado do cliente</span><span class="sxs-lookup"><span data-stu-id="e5577-127">Upload client certificate</span></span>](../api/identityapiconnector-uploadclientcertificate.md)|[<span data-ttu-id="e5577-128">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="e5577-128">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="e5577-129">Carregar um certificado de cliente a ser usado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="e5577-129">Upload a client certificate to use for authentication.</span></span>|
|[<span data-ttu-id="e5577-130">Delete</span><span class="sxs-lookup"><span data-stu-id="e5577-130">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="e5577-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5577-131">None</span></span>|<span data-ttu-id="e5577-132">Exclua um conector de API.</span><span class="sxs-lookup"><span data-stu-id="e5577-132">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5577-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e5577-133">Properties</span></span>

|<span data-ttu-id="e5577-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5577-134">Property</span></span>|<span data-ttu-id="e5577-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5577-135">Type</span></span>|<span data-ttu-id="e5577-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5577-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5577-137">id</span><span class="sxs-lookup"><span data-stu-id="e5577-137">id</span></span>|<span data-ttu-id="e5577-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5577-138">String</span></span>|<span data-ttu-id="e5577-139">A ID gerada aleatoriamente do conector da API.</span><span class="sxs-lookup"><span data-stu-id="e5577-139">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="e5577-140">displayName</span><span class="sxs-lookup"><span data-stu-id="e5577-140">displayName</span></span>|<span data-ttu-id="e5577-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5577-141">String</span></span>| <span data-ttu-id="e5577-142">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="e5577-142">The name of the API connector.</span></span> |
|<span data-ttu-id="e5577-143">targetUrl</span><span class="sxs-lookup"><span data-stu-id="e5577-143">targetUrl</span></span>|<span data-ttu-id="e5577-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5577-144">String</span></span>| <span data-ttu-id="e5577-145">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="e5577-145">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="e5577-146">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e5577-146">authenticationConfiguration</span></span>|[<span data-ttu-id="e5577-147">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="e5577-147">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="e5577-148">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="e5577-148">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="e5577-149">Certificado cliente básico e PKCS 12 são suportados.</span><span class="sxs-lookup"><span data-stu-id="e5577-149">Basic and PKCS 12 client certificate are supported.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5577-150">Relações</span><span class="sxs-lookup"><span data-stu-id="e5577-150">Relationships</span></span>

<span data-ttu-id="e5577-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e5577-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5577-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e5577-152">JSON representation</span></span>

<span data-ttu-id="e5577-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e5577-153">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityApiConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "targetUrl": "String",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
  }
}
```
