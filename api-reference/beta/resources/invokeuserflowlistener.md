---
title: Tipo de recurso invokeUserFlowListener
description: Um ouvinte usado para invocar um fluxo de usuário durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7eee91460c623be982cb316edae1c3c2f0734b07
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442989"
---
# <a name="invokeuserflowlistener-resource-type"></a><span data-ttu-id="70123-103">Tipo de recurso invokeUserFlowListener</span><span class="sxs-lookup"><span data-stu-id="70123-103">invokeUserFlowListener resource type</span></span>

<span data-ttu-id="70123-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70123-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70123-105">Você pode criar [um invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="70123-105">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event.</span></span> <span data-ttu-id="70123-106">Isso associa um aplicativo a um fluxo de usuário, que permite que identidades externas [se inscrevam](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70123-106">This associates an application with a user flow, which enables [external identities self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) for the application.</span></span> <span data-ttu-id="70123-107">Depois que um aplicativo é associado a um fluxo de usuários, os usuários que vão para esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.</span><span class="sxs-lookup"><span data-stu-id="70123-107">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

<span data-ttu-id="70123-108">Herda da autenticação de tipo base [abstrataListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="70123-108">Inherits from the abstract base type [authenticationListener](../resources/authenticationlistener.md).</span></span>

## <a name="properties"></a><span data-ttu-id="70123-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70123-109">Properties</span></span>

|<span data-ttu-id="70123-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70123-110">Property</span></span>|<span data-ttu-id="70123-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="70123-111">Type</span></span>|<span data-ttu-id="70123-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="70123-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70123-113">id</span><span class="sxs-lookup"><span data-stu-id="70123-113">id</span></span>|<span data-ttu-id="70123-114">String</span><span class="sxs-lookup"><span data-stu-id="70123-114">String</span></span>|<span data-ttu-id="70123-115">O identificador da ação.</span><span class="sxs-lookup"><span data-stu-id="70123-115">The identifier of the action.</span></span> <span data-ttu-id="70123-116">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="70123-116">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="70123-117">prioridade</span><span class="sxs-lookup"><span data-stu-id="70123-117">priority</span></span>|<span data-ttu-id="70123-118">Int32</span><span class="sxs-lookup"><span data-stu-id="70123-118">Int32</span></span>|<span data-ttu-id="70123-119">A prioridade da ação usada para determinar uma de várias ações aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="70123-119">The priority of the action that is used to determine one out of multiple applicable actions.</span></span> <span data-ttu-id="70123-120">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="70123-120">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="70123-121">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="70123-121">sourceFilter</span></span>|[<span data-ttu-id="70123-122">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="70123-122">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="70123-123">Filtrar com base na origem da autenticação usada para determinar se o ouvinte é executado.</span><span class="sxs-lookup"><span data-stu-id="70123-123">Filter based on the source of the authentication that is used to determine whether the listener is executed.</span></span> <span data-ttu-id="70123-124">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="70123-124">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="70123-125">Relações</span><span class="sxs-lookup"><span data-stu-id="70123-125">Relationships</span></span>

|<span data-ttu-id="70123-126">Relação</span><span class="sxs-lookup"><span data-stu-id="70123-126">Relationship</span></span>|<span data-ttu-id="70123-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="70123-127">Type</span></span>|<span data-ttu-id="70123-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="70123-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70123-129">userFlow</span><span class="sxs-lookup"><span data-stu-id="70123-129">userFlow</span></span>|[<span data-ttu-id="70123-130">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="70123-130">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="70123-131">O fluxo do usuário que é invocado quando essa ação é executada.</span><span class="sxs-lookup"><span data-stu-id="70123-131">The user flow that is invoked when this action executes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70123-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70123-132">JSON representation</span></span>

<span data-ttu-id="70123-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="70123-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.invokeUserFlowListener",
  "baseType": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  },
  "userFlow": {
    "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
  }
}
```
