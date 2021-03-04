---
title: Tipo de recurso authenticationListener
description: Define o ouvinte a ser avaliada durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a7feeabaa9caf0246a53aded7ac1c15236fdf8af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433177"
---
# <a name="authenticationlistener-resource-type"></a><span data-ttu-id="545f6-103">Tipo de recurso authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-103">authenticationListener resource type</span></span>

<span data-ttu-id="545f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="545f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="545f6-105">Define um ouvinte a ser avaliada quando um evento de autenticação acontece em uma experiência de autenticação.</span><span class="sxs-lookup"><span data-stu-id="545f6-105">Defines a listener to be evaluate when an authentication event happens in an authentication experience.</span></span> <span data-ttu-id="545f6-106">Um authenticationListener é abstrato e é a classe base dos vários tipos de ouvintes que você pode avaliar durante um evento de autenticação.</span><span class="sxs-lookup"><span data-stu-id="545f6-106">An authenticationListener is abstract and is the base class of the various types of listeners you can evaluate during an authentication event.</span></span> 

<span data-ttu-id="545f6-107">Você pode criar [um invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart..</span><span class="sxs-lookup"><span data-stu-id="545f6-107">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event..</span></span> <span data-ttu-id="545f6-108">Isso associa um aplicativo a um fluxo de usuário, portanto, habilitando um processo de [inscrição de autoatendenciamento.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview)</span><span class="sxs-lookup"><span data-stu-id="545f6-108">This associates an application with a user flow, therefore enabling a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) process.</span></span> <span data-ttu-id="545f6-109">Depois que um aplicativo é associado a um fluxo de usuários, os usuários que vão para esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.</span><span class="sxs-lookup"><span data-stu-id="545f6-109">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

## <a name="methods"></a><span data-ttu-id="545f6-110">Methods</span><span class="sxs-lookup"><span data-stu-id="545f6-110">Methods</span></span>

|<span data-ttu-id="545f6-111">Método</span><span class="sxs-lookup"><span data-stu-id="545f6-111">Method</span></span>|<span data-ttu-id="545f6-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="545f6-112">Return type</span></span>|<span data-ttu-id="545f6-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="545f6-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="545f6-114">Listar onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="545f6-114">List onSignUpStart</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="545f6-115">[Coleção authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="545f6-115">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="545f6-116">Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="545f6-116">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="545f6-117">Criar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-117">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="545f6-118">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-118">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="545f6-119">Crie um novo objeto authenticationListener para o evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="545f6-119">Create a new authenticationListener object for the onSignupStart event.</span></span>|
|[<span data-ttu-id="545f6-120">Atualizar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-120">Update authenticationListener</span></span>](../api/authenticationlistener-update.md)|[<span data-ttu-id="545f6-121">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-121">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="545f6-122">Atualize o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="545f6-122">Update the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="545f6-123">Colocar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-123">Put authenticationListener</span></span>](../api/authenticationlistener-put.md)|[<span data-ttu-id="545f6-124">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-124">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="545f6-125">Substitua as propriedades de um objeto authenticationListener.</span><span class="sxs-lookup"><span data-stu-id="545f6-125">Replace the properties of an authenticationListener object.</span></span>|
|[<span data-ttu-id="545f6-126">Obter authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-126">Get authenticationListener</span></span>](../api/authenticationlistener-get.md)|[<span data-ttu-id="545f6-127">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-127">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="545f6-128">Obter o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="545f6-128">Get the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="545f6-129">Excluir authenticationListener</span><span class="sxs-lookup"><span data-stu-id="545f6-129">Delete authenticationListener</span></span>](../api/authenticationlistener-delete.md)|<span data-ttu-id="545f6-130">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="545f6-130">None</span></span>|<span data-ttu-id="545f6-131">Exclua o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="545f6-131">Delete the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|

## <a name="properties"></a><span data-ttu-id="545f6-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="545f6-132">Properties</span></span>

|<span data-ttu-id="545f6-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="545f6-133">Property</span></span>|<span data-ttu-id="545f6-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="545f6-134">Type</span></span>|<span data-ttu-id="545f6-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="545f6-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="545f6-136">id</span><span class="sxs-lookup"><span data-stu-id="545f6-136">id</span></span>|<span data-ttu-id="545f6-137">String</span><span class="sxs-lookup"><span data-stu-id="545f6-137">String</span></span>|<span data-ttu-id="545f6-138">O identificador da ação.</span><span class="sxs-lookup"><span data-stu-id="545f6-138">The identifier of the action.</span></span>|
|<span data-ttu-id="545f6-139">prioridade</span><span class="sxs-lookup"><span data-stu-id="545f6-139">priority</span></span>|<span data-ttu-id="545f6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="545f6-140">Int32</span></span>|<span data-ttu-id="545f6-141">A prioridade do ouvinte.</span><span class="sxs-lookup"><span data-stu-id="545f6-141">The priority of the listener.</span></span> <span data-ttu-id="545f6-142">Determina a ordem de avaliação quando um evento tem vários ouvintes.</span><span class="sxs-lookup"><span data-stu-id="545f6-142">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="545f6-143">A prioridade é avaliada de baixo para alto.</span><span class="sxs-lookup"><span data-stu-id="545f6-143">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="545f6-144">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="545f6-144">sourceFilter</span></span>|[<span data-ttu-id="545f6-145">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="545f6-145">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="545f6-146">Filtrar com base na origem da autenticação usada para determinar se o ouvinte é avaliado.</span><span class="sxs-lookup"><span data-stu-id="545f6-146">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="545f6-147">No momento, isso está limitado a avaliações com base no aplicativo ao que o usuário está autenticando.</span><span class="sxs-lookup"><span data-stu-id="545f6-147">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="545f6-148">Relações</span><span class="sxs-lookup"><span data-stu-id="545f6-148">Relationships</span></span>

<span data-ttu-id="545f6-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="545f6-149">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="545f6-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="545f6-150">JSON representation</span></span>

<span data-ttu-id="545f6-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="545f6-151">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  }
}
```
