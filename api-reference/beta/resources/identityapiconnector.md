---
title: Tipo de recurso identityApiConnector
description: Representa conectores de API em um locatário do Azure Active Directory.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e5b3c10e6a03c4868e010f8f62f0f073ce37ca61
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161646"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="6da72-103">Tipo de recurso identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="6da72-103">identityApiConnector resource type</span></span>

<span data-ttu-id="6da72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6da72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6da72-105">Representa conectores de API em um Azure Active Directory (Azure AD) e locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="6da72-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="6da72-106">Um conector de API usado em sua assinatura de identidades externas do Azure AD e fluxos de usuário de assinatura do Azure AD B2C permite que você chame uma API durante a execução do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6da72-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="6da72-107">Um conector de API fornece as informações necessárias para chamar uma API, incluindo uma URL de ponto de extremidade e autenticação.</span><span class="sxs-lookup"><span data-stu-id="6da72-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="6da72-108">Um conector de API pode ser usado em uma etapa específica em um fluxo de usuário para afetar a execução do fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="6da72-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="6da72-109">Por exemplo, a resposta da API pode impedir que um usuário se inscreve, mostrar um erro de validação de entrada ou substituir atributos coletados pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="6da72-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="6da72-110">Use a API [b2xIdentityUserFlow](b2xidentityuserflow.md) para usar um conector de API de um fluxo de usuário de entrada de autoatendente identidades externas.</span><span class="sxs-lookup"><span data-stu-id="6da72-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="6da72-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="6da72-111">Methods</span></span>

|<span data-ttu-id="6da72-112">Método</span><span class="sxs-lookup"><span data-stu-id="6da72-112">Method</span></span>|<span data-ttu-id="6da72-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6da72-113">Return type</span></span>|<span data-ttu-id="6da72-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da72-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6da72-115">List</span><span class="sxs-lookup"><span data-stu-id="6da72-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="6da72-116">[Coleção identityApiConnector](identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="6da72-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="6da72-117">Obter uma lista de conectores de API</span><span class="sxs-lookup"><span data-stu-id="6da72-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="6da72-118">Criar</span><span class="sxs-lookup"><span data-stu-id="6da72-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="6da72-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="6da72-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="6da72-120">Crie um novo conector de API.</span><span class="sxs-lookup"><span data-stu-id="6da72-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="6da72-121">Get</span><span class="sxs-lookup"><span data-stu-id="6da72-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="6da72-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="6da72-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="6da72-123">Leia as propriedades de um [objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="6da72-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="6da72-124">Update</span><span class="sxs-lookup"><span data-stu-id="6da72-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="6da72-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="6da72-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="6da72-126">Atualizar as propriedades de um conector de API.</span><span class="sxs-lookup"><span data-stu-id="6da72-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="6da72-127">Delete</span><span class="sxs-lookup"><span data-stu-id="6da72-127">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="6da72-128">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="6da72-128">None</span></span>|<span data-ttu-id="6da72-129">Exclua um conector de API.</span><span class="sxs-lookup"><span data-stu-id="6da72-129">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="6da72-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6da72-130">Properties</span></span>

|<span data-ttu-id="6da72-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6da72-131">Property</span></span>|<span data-ttu-id="6da72-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6da72-132">Type</span></span>|<span data-ttu-id="6da72-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6da72-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da72-134">id</span><span class="sxs-lookup"><span data-stu-id="6da72-134">id</span></span>|<span data-ttu-id="6da72-135">String</span><span class="sxs-lookup"><span data-stu-id="6da72-135">String</span></span>|<span data-ttu-id="6da72-136">A ID gerada aleatoriamente do conector da API.</span><span class="sxs-lookup"><span data-stu-id="6da72-136">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="6da72-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6da72-137">displayName</span></span>|<span data-ttu-id="6da72-138">String</span><span class="sxs-lookup"><span data-stu-id="6da72-138">String</span></span>| <span data-ttu-id="6da72-139">O nome do conector da API.</span><span class="sxs-lookup"><span data-stu-id="6da72-139">The name of the API connector.</span></span> |
|<span data-ttu-id="6da72-140">targetUrl</span><span class="sxs-lookup"><span data-stu-id="6da72-140">targetUrl</span></span>|<span data-ttu-id="6da72-141">String</span><span class="sxs-lookup"><span data-stu-id="6da72-141">String</span></span>| <span data-ttu-id="6da72-142">A URL do ponto de extremidade da API a ser chamada.</span><span class="sxs-lookup"><span data-stu-id="6da72-142">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="6da72-143">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6da72-143">authenticationConfiguration</span></span>|[<span data-ttu-id="6da72-144">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="6da72-144">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="6da72-145">O objeto que descreve os detalhes de configuração de autenticação para chamar a API.</span><span class="sxs-lookup"><span data-stu-id="6da72-145">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="6da72-146">Somente [a autenticação](basicauthentication.md) Básica é suportada no momento.</span><span class="sxs-lookup"><span data-stu-id="6da72-146">Only [Basic authentication](basicauthentication.md) is supported at this time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6da72-147">Relações</span><span class="sxs-lookup"><span data-stu-id="6da72-147">Relationships</span></span>

<span data-ttu-id="6da72-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6da72-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6da72-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6da72-149">JSON representation</span></span>

<span data-ttu-id="6da72-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6da72-150">The following is a JSON representation of the resource.</span></span>
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
