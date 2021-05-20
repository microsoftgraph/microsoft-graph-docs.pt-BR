---
title: Tipo de recurso invokeUserFlowListener
description: Um ouvinte usado para invocar um fluxo de usuário durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 89f990ab4692ec7fd4d6ce3b94ee4c4d4846c6c4
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547208"
---
# <a name="invokeuserflowlistener-resource-type"></a><span data-ttu-id="bdf68-103">Tipo de recurso invokeUserFlowListener</span><span class="sxs-lookup"><span data-stu-id="bdf68-103">invokeUserFlowListener resource type</span></span>

<span data-ttu-id="bdf68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdf68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf68-105">Você pode criar [um invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="bdf68-105">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event.</span></span> <span data-ttu-id="bdf68-106">Isso associa um aplicativo a um fluxo de usuário, que permite que identidades externas [se inscrevam](/azure/active-directory/external-identities/self-service-sign-up-overview) no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bdf68-106">This associates an application with a user flow, which enables [external identities self-service sign up](/azure/active-directory/external-identities/self-service-sign-up-overview) for the application.</span></span> <span data-ttu-id="bdf68-107">Depois que um aplicativo é associado a um fluxo de usuários, os usuários que vão para esse aplicativo poderão iniciar um fluxo de inscrição que provisiona uma conta de convidado.</span><span class="sxs-lookup"><span data-stu-id="bdf68-107">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

<span data-ttu-id="bdf68-108">Herda da autenticação de tipo base [abstrataListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="bdf68-108">Inherits from the abstract base type [authenticationListener](../resources/authenticationlistener.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bdf68-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdf68-109">Properties</span></span>

|<span data-ttu-id="bdf68-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdf68-110">Property</span></span>|<span data-ttu-id="bdf68-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf68-111">Type</span></span>|<span data-ttu-id="bdf68-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf68-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf68-113">id</span><span class="sxs-lookup"><span data-stu-id="bdf68-113">id</span></span>|<span data-ttu-id="bdf68-114">String</span><span class="sxs-lookup"><span data-stu-id="bdf68-114">String</span></span>|<span data-ttu-id="bdf68-115">O identificador da ação.</span><span class="sxs-lookup"><span data-stu-id="bdf68-115">The identifier of the action.</span></span> <span data-ttu-id="bdf68-116">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="bdf68-116">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="bdf68-117">prioridade</span><span class="sxs-lookup"><span data-stu-id="bdf68-117">priority</span></span>|<span data-ttu-id="bdf68-118">Int32</span><span class="sxs-lookup"><span data-stu-id="bdf68-118">Int32</span></span>|<span data-ttu-id="bdf68-119">A prioridade da ação usada para determinar uma de várias ações aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="bdf68-119">The priority of the action that is used to determine one out of multiple applicable actions.</span></span> <span data-ttu-id="bdf68-120">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="bdf68-120">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="bdf68-121">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="bdf68-121">sourceFilter</span></span>|[<span data-ttu-id="bdf68-122">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="bdf68-122">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="bdf68-123">Filtrar com base na origem da autenticação usada para determinar se o ouvinte é executado.</span><span class="sxs-lookup"><span data-stu-id="bdf68-123">Filter based on the source of the authentication that is used to determine whether the listener is executed.</span></span> <span data-ttu-id="bdf68-124">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="bdf68-124">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdf68-125">Relações</span><span class="sxs-lookup"><span data-stu-id="bdf68-125">Relationships</span></span>

|<span data-ttu-id="bdf68-126">Relação</span><span class="sxs-lookup"><span data-stu-id="bdf68-126">Relationship</span></span>|<span data-ttu-id="bdf68-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf68-127">Type</span></span>|<span data-ttu-id="bdf68-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf68-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdf68-129">userFlow</span><span class="sxs-lookup"><span data-stu-id="bdf68-129">userFlow</span></span>|[<span data-ttu-id="bdf68-130">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="bdf68-130">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="bdf68-131">O fluxo do usuário que é invocado quando essa ação é executada.</span><span class="sxs-lookup"><span data-stu-id="bdf68-131">The user flow that is invoked when this action executes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdf68-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdf68-132">JSON representation</span></span>

<span data-ttu-id="bdf68-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdf68-133">The following is a JSON representation of the resource.</span></span>
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
