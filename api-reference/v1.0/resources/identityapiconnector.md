---
title: Tipo de recurso identityApiConnector
description: Representa conectores de API em um locatário do Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8fc0ff1915bd76a35d9eb0c0041e1628fde41981
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882763"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="24b7f-103">Tipo de recurso identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="24b7f-103">identityApiConnector resource type</span></span>

<span data-ttu-id="24b7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24b7f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24b7f-105">Representa conectores de API em locatários do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="24b7f-105">Represents API connectors in an Azure Active Directory (Azure AD) tenants.</span></span>

<span data-ttu-id="24b7f-106">Um conector de API usado em seus fluxos de usuário de autoatendados de identidades externas do Azure AD permite que você chame uma API durante a execução do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="24b7f-106">An API connector used in your Azure AD External Identities self-service sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="24b7f-107">Um conector de API fornece as informações necessárias para chamar uma API, incluindo uma URL de ponto de extremidade e autenticação.</span><span class="sxs-lookup"><span data-stu-id="24b7f-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="24b7f-108">Um conector de API pode ser usado em uma etapa específica em um fluxo de usuário para afetar a execução do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="24b7f-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="24b7f-109">Por exemplo, a resposta da API pode impedir que um usuário se inscreve, mostrar um erro de validação de entrada ou substituir atributos coletados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="24b7f-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="24b7f-110">Use a [API b2xIdentityUserFlow](b2xidentityuserflow.md) para usar um conector de API de um fluxo de usuário de autoatendência de Identidades Externas.</span><span class="sxs-lookup"><span data-stu-id="24b7f-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="24b7f-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="24b7f-111">Methods</span></span>

|<span data-ttu-id="24b7f-112">Método</span><span class="sxs-lookup"><span data-stu-id="24b7f-112">Method</span></span>|<span data-ttu-id="24b7f-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="24b7f-113">Return type</span></span>|<span data-ttu-id="24b7f-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="24b7f-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24b7f-115">List</span><span class="sxs-lookup"><span data-stu-id="24b7f-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="24b7f-116">[Coleção identityApiConnector](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="24b7f-116">[identityApiConnector](../resources/identityapiconnector.md) collection</span></span>| <span data-ttu-id="24b7f-117">Obter uma lista de conectores de API</span><span class="sxs-lookup"><span data-stu-id="24b7f-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="24b7f-118">Create</span><span class="sxs-lookup"><span data-stu-id="24b7f-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="24b7f-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="24b7f-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="24b7f-120">Crie um novo conector de API.</span><span class="sxs-lookup"><span data-stu-id="24b7f-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="24b7f-121">Get</span><span class="sxs-lookup"><span data-stu-id="24b7f-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="24b7f-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="24b7f-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="24b7f-123">Leia as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="24b7f-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="24b7f-124">Atualizar</span><span class="sxs-lookup"><span data-stu-id="24b7f-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="24b7f-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="24b7f-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="24b7f-126">Atualize as propriedades de um conector de API.</span><span class="sxs-lookup"><span data-stu-id="24b7f-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="24b7f-127">Carregar certificado do cliente</span><span class="sxs-lookup"><span data-stu-id="24b7f-127">Upload client certificate</span></span>](../api/identityapiconnector-uploadclientcertificate.md)|[<span data-ttu-id="24b7f-128">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="24b7f-128">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="24b7f-129">Carregar um certificado de cliente a ser usado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="24b7f-129">Upload a client certificate to use for authentication.</span></span>|
|[<span data-ttu-id="24b7f-130">Delete</span><span class="sxs-lookup"><span data-stu-id="24b7f-130">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="24b7f-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24b7f-131">None</span></span>|<span data-ttu-id="24b7f-132">Exclua um conector de API.</span><span class="sxs-lookup"><span data-stu-id="24b7f-132">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="24b7f-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24b7f-133">Properties</span></span>

|<span data-ttu-id="24b7f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24b7f-134">Property</span></span>|<span data-ttu-id="24b7f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="24b7f-135">Type</span></span>|<span data-ttu-id="24b7f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="24b7f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b7f-137">id</span><span class="sxs-lookup"><span data-stu-id="24b7f-137">id</span></span>|<span data-ttu-id="24b7f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24b7f-138">String</span></span>|<span data-ttu-id="24b7f-139">O identificador gerado aleatoriamente do conector de API.</span><span class="sxs-lookup"><span data-stu-id="24b7f-139">The randomly generated identifier of the API connector.</span></span> |
|<span data-ttu-id="24b7f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="24b7f-140">displayName</span></span>|<span data-ttu-id="24b7f-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24b7f-141">String</span></span>| <span data-ttu-id="24b7f-142">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="24b7f-142">The name of the API connector.</span></span> |
|<span data-ttu-id="24b7f-143">targetUrl</span><span class="sxs-lookup"><span data-stu-id="24b7f-143">targetUrl</span></span>|<span data-ttu-id="24b7f-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24b7f-144">String</span></span>| <span data-ttu-id="24b7f-145">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="24b7f-145">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="24b7f-146">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="24b7f-146">authenticationConfiguration</span></span>|[<span data-ttu-id="24b7f-147">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="24b7f-147">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="24b7f-148">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="24b7f-148">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="24b7f-149">Certificado cliente básico e PKCS 12 são suportados.</span><span class="sxs-lookup"><span data-stu-id="24b7f-149">Basic and PKCS 12 client certificate are supported.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24b7f-150">Relações</span><span class="sxs-lookup"><span data-stu-id="24b7f-150">Relationships</span></span>

<span data-ttu-id="24b7f-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24b7f-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24b7f-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24b7f-152">JSON representation</span></span>

<span data-ttu-id="24b7f-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="24b7f-153">The following is a JSON representation of the resource.</span></span>
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
