---
title: tipo de recurso identityApiConnector
description: Representa conectores de API em um locatário do Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6098b146b5117332df36b76adcbce95698d6041d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720096"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="7bae6-103">tipo de recurso identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="7bae6-103">identityApiConnector resource type</span></span>

<span data-ttu-id="7bae6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bae6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bae6-105">Representa os conectores de API em um Azure Active Directory (Azure AD) e locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="7bae6-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="7bae6-106">Um conector de API usado em suas identidades externas do Azure AD inscrição de autoatendimento e os fluxos de usuário de inscrição do Azure AD B2C permitem chamar uma API durante a execução do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="7bae6-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="7bae6-107">Um conector de API fornece as informações necessárias para chamar uma API, incluindo uma URL de ponto de extremidade e autenticação.</span><span class="sxs-lookup"><span data-stu-id="7bae6-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="7bae6-108">Um conector de API pode ser usado em uma etapa específica em um fluxo de usuário para afetar a execução do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="7bae6-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="7bae6-109">Por exemplo, a resposta da API pode impedir que um usuário se inscrever, mostrar um erro de validação de entrada ou substituir os atributos coletados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="7bae6-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="7bae6-110">Use a API [b2xIdentityUserFlow](b2xidentityuserflow.md) para usar um conector de API de um fluxo de usuário de inscrição de autoatendimento de identidade externa.</span><span class="sxs-lookup"><span data-stu-id="7bae6-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="7bae6-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="7bae6-111">Methods</span></span>

|<span data-ttu-id="7bae6-112">Método</span><span class="sxs-lookup"><span data-stu-id="7bae6-112">Method</span></span>|<span data-ttu-id="7bae6-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7bae6-113">Return type</span></span>|<span data-ttu-id="7bae6-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bae6-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7bae6-115">List</span><span class="sxs-lookup"><span data-stu-id="7bae6-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="7bae6-116">coleção [identityApiConnector](identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="7bae6-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="7bae6-117">Obter uma lista de conectores de API</span><span class="sxs-lookup"><span data-stu-id="7bae6-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="7bae6-118">Create</span><span class="sxs-lookup"><span data-stu-id="7bae6-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="7bae6-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="7bae6-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="7bae6-120">Criar um novo conector de API.</span><span class="sxs-lookup"><span data-stu-id="7bae6-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="7bae6-121">Get</span><span class="sxs-lookup"><span data-stu-id="7bae6-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="7bae6-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="7bae6-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="7bae6-123">Ler as propriedades de um objeto [identityApiConnector](../resources/identityapiconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="7bae6-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="7bae6-124">Update</span><span class="sxs-lookup"><span data-stu-id="7bae6-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="7bae6-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="7bae6-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="7bae6-126">Atualizar as propriedades de um conector de API.</span><span class="sxs-lookup"><span data-stu-id="7bae6-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="7bae6-127">Delete</span><span class="sxs-lookup"><span data-stu-id="7bae6-127">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="7bae6-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bae6-128">None</span></span>|<span data-ttu-id="7bae6-129">Excluir um conector de API.</span><span class="sxs-lookup"><span data-stu-id="7bae6-129">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="7bae6-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bae6-130">Properties</span></span>

|<span data-ttu-id="7bae6-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bae6-131">Property</span></span>|<span data-ttu-id="7bae6-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bae6-132">Type</span></span>|<span data-ttu-id="7bae6-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bae6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bae6-134">id</span><span class="sxs-lookup"><span data-stu-id="7bae6-134">id</span></span>|<span data-ttu-id="7bae6-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bae6-135">String</span></span>|<span data-ttu-id="7bae6-136">A ID gerada aleatoriamente do conector da API.</span><span class="sxs-lookup"><span data-stu-id="7bae6-136">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="7bae6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7bae6-137">displayName</span></span>|<span data-ttu-id="7bae6-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bae6-138">String</span></span>| <span data-ttu-id="7bae6-139">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="7bae6-139">The name of the API connector.</span></span> |
|<span data-ttu-id="7bae6-140">targetUrl</span><span class="sxs-lookup"><span data-stu-id="7bae6-140">targetUrl</span></span>|<span data-ttu-id="7bae6-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bae6-141">String</span></span>| <span data-ttu-id="7bae6-142">A URL do ponto de extremidade da API a ser chamado.</span><span class="sxs-lookup"><span data-stu-id="7bae6-142">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="7bae6-143">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7bae6-143">authenticationConfiguration</span></span>|[<span data-ttu-id="7bae6-144">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="7bae6-144">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="7bae6-145">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="7bae6-145">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="7bae6-146">Só há suporte para a [autenticação básica](basicauthentication.md) no momento.</span><span class="sxs-lookup"><span data-stu-id="7bae6-146">Only [Basic authentication](basicauthentication.md) is supported at this time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bae6-147">Relações</span><span class="sxs-lookup"><span data-stu-id="7bae6-147">Relationships</span></span>

<span data-ttu-id="7bae6-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bae6-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bae6-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bae6-149">JSON representation</span></span>

<span data-ttu-id="7bae6-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bae6-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "baseType": "",
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
