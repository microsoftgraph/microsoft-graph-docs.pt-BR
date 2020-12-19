---
title: tipo de recurso invokeUserFlowListener
description: Um ouvinte usado para invocar um fluxo de usuário durante um evento de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ca1c61d830a2ff98f2d72839129d75cc6287c36
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720089"
---
# <a name="invokeuserflowlistener-resource-type"></a><span data-ttu-id="014d9-103">tipo de recurso invokeUserFlowListener</span><span class="sxs-lookup"><span data-stu-id="014d9-103">invokeUserFlowListener resource type</span></span>

<span data-ttu-id="014d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="014d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="014d9-105">Você pode criar um [invokeUserFlowListener](../resources/invokeuserflowlistener.md) para o evento onSignUpStart.</span><span class="sxs-lookup"><span data-stu-id="014d9-105">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event.</span></span> <span data-ttu-id="014d9-106">Isso associa um aplicativo a um fluxo de usuário, que permite a [inscrição de autoatendimento de identidade externa](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="014d9-106">This associates an application with a user flow, which enables [external identities self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) for the application.</span></span> <span data-ttu-id="014d9-107">Depois que um aplicativo é associado a um fluxo de usuário, os usuários que acessam esse aplicativo poderão iniciar um fluxo de inscrição que Provisione uma conta de convidado.</span><span class="sxs-lookup"><span data-stu-id="014d9-107">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

<span data-ttu-id="014d9-108">Herda do tipo de base abstrato [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="014d9-108">Inherits from the abstract base type [authenticationListener](../resources/authenticationlistener.md).</span></span>

## <a name="properties"></a><span data-ttu-id="014d9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="014d9-109">Properties</span></span>

|<span data-ttu-id="014d9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="014d9-110">Property</span></span>|<span data-ttu-id="014d9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="014d9-111">Type</span></span>|<span data-ttu-id="014d9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="014d9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="014d9-113">id</span><span class="sxs-lookup"><span data-stu-id="014d9-113">id</span></span>|<span data-ttu-id="014d9-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="014d9-114">String</span></span>|<span data-ttu-id="014d9-115">O identificador da ação.</span><span class="sxs-lookup"><span data-stu-id="014d9-115">The identifier of the action.</span></span> <span data-ttu-id="014d9-116">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="014d9-116">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="014d9-117">prioridade</span><span class="sxs-lookup"><span data-stu-id="014d9-117">priority</span></span>|<span data-ttu-id="014d9-118">Int32</span><span class="sxs-lookup"><span data-stu-id="014d9-118">Int32</span></span>|<span data-ttu-id="014d9-119">A prioridade da ação que é usada para determinar uma de várias ações aplicáveis.</span><span class="sxs-lookup"><span data-stu-id="014d9-119">The priority of the action that is used to determine one out of multiple applicable actions.</span></span> <span data-ttu-id="014d9-120">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="014d9-120">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="014d9-121">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="014d9-121">sourceFilter</span></span>|[<span data-ttu-id="014d9-122">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="014d9-122">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="014d9-123">Filtro com base na origem da autenticação que é usada para determinar se o ouvinte é executado.</span><span class="sxs-lookup"><span data-stu-id="014d9-123">Filter based on the source of the authentication that is used to determine whether the listener is executed.</span></span> <span data-ttu-id="014d9-124">Herdado de [authenticationListener](../resources/authenticationlistener.md).</span><span class="sxs-lookup"><span data-stu-id="014d9-124">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="014d9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="014d9-125">Relationships</span></span>

|<span data-ttu-id="014d9-126">Relação</span><span class="sxs-lookup"><span data-stu-id="014d9-126">Relationship</span></span>|<span data-ttu-id="014d9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="014d9-127">Type</span></span>|<span data-ttu-id="014d9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="014d9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="014d9-129">userflow</span><span class="sxs-lookup"><span data-stu-id="014d9-129">userFlow</span></span>|[<span data-ttu-id="014d9-130">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="014d9-130">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="014d9-131">O fluxo do usuário que é chamado quando esta ação é executada.</span><span class="sxs-lookup"><span data-stu-id="014d9-131">The user flow that is invoked when this action executes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="014d9-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="014d9-132">JSON representation</span></span>

<span data-ttu-id="014d9-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="014d9-133">The following is a JSON representation of the resource.</span></span>
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
