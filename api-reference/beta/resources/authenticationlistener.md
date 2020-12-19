---
title: tipo de recurso authenticationListener
description: Define o ouvinte a ser avaliado durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d89d7660fc2580b8fad185633b6b819df1a41aaf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720061"
---
# <a name="authenticationlistener-resource-type"></a><span data-ttu-id="0b677-103">tipo de recurso authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-103">authenticationListener resource type</span></span>

<span data-ttu-id="0b677-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b677-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b677-105">Define um ouvinte a ser avaliado quando um evento de autenticação ocorrer em uma experiência de autenticação.</span><span class="sxs-lookup"><span data-stu-id="0b677-105">Defines a listener to be evaluate when an authentication event happens in an authentication experience.</span></span> <span data-ttu-id="0b677-106">Um authenticationListener é abstrato e é a classe base dos vários tipos de ouvintes que você pode avaliar durante um evento de autenticação.</span><span class="sxs-lookup"><span data-stu-id="0b677-106">An authenticationListener is abstract and is the base class of the various types of listeners you can evaluate during an authentication event.</span></span> 

<span data-ttu-id="0b677-107">Você pode criar um [invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart..</span><span class="sxs-lookup"><span data-stu-id="0b677-107">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event..</span></span> <span data-ttu-id="0b677-108">Isso associa um aplicativo a um fluxo de usuário, habilitando, portanto, o processo de [inscrição de autoatendimento](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) .</span><span class="sxs-lookup"><span data-stu-id="0b677-108">This associates an application with a user flow, therefore enabling a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) process.</span></span> <span data-ttu-id="0b677-109">Depois que um aplicativo é associado a um fluxo de usuário, os usuários que acessam esse aplicativo poderão iniciar um fluxo de inscrição que Provisione uma conta de convidado.</span><span class="sxs-lookup"><span data-stu-id="0b677-109">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

## <a name="methods"></a><span data-ttu-id="0b677-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b677-110">Methods</span></span>

|<span data-ttu-id="0b677-111">Método</span><span class="sxs-lookup"><span data-stu-id="0b677-111">Method</span></span>|<span data-ttu-id="0b677-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0b677-112">Return type</span></span>|<span data-ttu-id="0b677-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b677-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0b677-114">Listar onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="0b677-114">List onSignUpStart</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="0b677-115">coleção [authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="0b677-115">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="0b677-116">Obtenha a coleção de recursos authenticationListener com suporte pelo evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="0b677-116">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="0b677-117">Criar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-117">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="0b677-118">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-118">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="0b677-119">Criar um novo objeto authenticationListener para o evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="0b677-119">Create a new authenticationListener object for the onSignupStart event.</span></span>|
|[<span data-ttu-id="0b677-120">Atualizar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-120">Update authenticationListener</span></span>](../api/authenticationlistener-update.md)|[<span data-ttu-id="0b677-121">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-121">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="0b677-122">Atualize o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="0b677-122">Update the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="0b677-123">Colocar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-123">Put authenticationListener</span></span>](../api/authenticationlistener-put.md)|[<span data-ttu-id="0b677-124">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-124">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="0b677-125">Substitua as propriedades de um objeto authenticationListener.</span><span class="sxs-lookup"><span data-stu-id="0b677-125">Replace the properties of an authenticationListener object.</span></span>|
|[<span data-ttu-id="0b677-126">Obter authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-126">Get authenticationListener</span></span>](../api/authenticationlistener-get.md)|[<span data-ttu-id="0b677-127">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-127">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="0b677-128">Obtenha o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="0b677-128">Get the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="0b677-129">Excluir authenticationListener</span><span class="sxs-lookup"><span data-stu-id="0b677-129">Delete authenticationListener</span></span>](../api/authenticationlistener-delete.md)|<span data-ttu-id="0b677-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b677-130">None</span></span>|<span data-ttu-id="0b677-131">Exclua o ouvinte especificado definido para o evento onSignupStart no pipeline de autenticação.</span><span class="sxs-lookup"><span data-stu-id="0b677-131">Delete the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b677-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b677-132">Properties</span></span>

|<span data-ttu-id="0b677-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b677-133">Property</span></span>|<span data-ttu-id="0b677-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b677-134">Type</span></span>|<span data-ttu-id="0b677-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b677-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b677-136">id</span><span class="sxs-lookup"><span data-stu-id="0b677-136">id</span></span>|<span data-ttu-id="0b677-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b677-137">String</span></span>|<span data-ttu-id="0b677-138">O identificador da ação.</span><span class="sxs-lookup"><span data-stu-id="0b677-138">The identifier of the action.</span></span>|
|<span data-ttu-id="0b677-139">prioridade</span><span class="sxs-lookup"><span data-stu-id="0b677-139">priority</span></span>|<span data-ttu-id="0b677-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0b677-140">Int32</span></span>|<span data-ttu-id="0b677-141">A prioridade do ouvinte.</span><span class="sxs-lookup"><span data-stu-id="0b677-141">The priority of the listener.</span></span> <span data-ttu-id="0b677-142">Determina a ordem de avaliação quando um evento tem vários ouvintes.</span><span class="sxs-lookup"><span data-stu-id="0b677-142">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="0b677-143">A prioridade é avaliada de baixo para alto.</span><span class="sxs-lookup"><span data-stu-id="0b677-143">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="0b677-144">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="0b677-144">sourceFilter</span></span>|[<span data-ttu-id="0b677-145">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="0b677-145">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="0b677-146">Filtro com base na origem da autenticação que é usada para determinar se o ouvinte é avaliado.</span><span class="sxs-lookup"><span data-stu-id="0b677-146">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="0b677-147">No momento, isso está limitado a avaliações com base no aplicativo para o qual o usuário está se Autenticando.</span><span class="sxs-lookup"><span data-stu-id="0b677-147">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b677-148">Relações</span><span class="sxs-lookup"><span data-stu-id="0b677-148">Relationships</span></span>

<span data-ttu-id="0b677-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b677-149">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b677-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b677-150">JSON representation</span></span>

<span data-ttu-id="0b677-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b677-151">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "baseType": "",
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
