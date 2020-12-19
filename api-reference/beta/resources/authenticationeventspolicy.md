---
title: tipo de recurso authenticationEventsPolicy
description: Eventos de autenticação são usados para invocar fluxos de usuário em pontos específicos no fluxo de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cc8789fb0de21980571bdcb5254a7760045e61b0
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720062"
---
# <a name="authenticationeventspolicy-resource-type"></a><span data-ttu-id="88863-103">tipo de recurso authenticationEventsPolicy</span><span class="sxs-lookup"><span data-stu-id="88863-103">authenticationEventsPolicy resource type</span></span>

<span data-ttu-id="88863-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88863-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88863-105">Um recurso que especifica os eventos na experiência de autenticação, com cada evento definindo mais detalhadamente os tipos de ouvintes disponíveis que podem ser criados para o evento.</span><span class="sxs-lookup"><span data-stu-id="88863-105">A resource that specifies the events in the authentication experience, with each event further defining the available types of listeners that can be created for the event.</span></span> <span data-ttu-id="88863-106">Os eventos são inerentes à experiência de autenticação; Este recurso não é configurável pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="88863-106">Events are inherent to the authentication experience; this resource is not user configurable.</span></span>

## <a name="methods"></a><span data-ttu-id="88863-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="88863-107">Methods</span></span>

|<span data-ttu-id="88863-108">Método</span><span class="sxs-lookup"><span data-stu-id="88863-108">Method</span></span>|<span data-ttu-id="88863-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="88863-109">Return type</span></span>|<span data-ttu-id="88863-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="88863-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88863-111">Listar ouvintes onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="88863-111">List onSignUpStart listeners</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="88863-112">coleção [authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="88863-112">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="88863-113">Obtenha a coleção de recursos authenticationListener com suporte pelo evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="88863-113">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="88863-114">Criar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="88863-114">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="88863-115">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="88863-115">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="88863-116">Criar um novo objeto authenticationListener para o evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="88863-116">Create a new authenticationListener object for the onSignupStart event.</span></span>|

## <a name="properties"></a><span data-ttu-id="88863-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88863-117">Properties</span></span>

|<span data-ttu-id="88863-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88863-118">Property</span></span>|<span data-ttu-id="88863-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="88863-119">Type</span></span>|<span data-ttu-id="88863-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="88863-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88863-121">id</span><span class="sxs-lookup"><span data-stu-id="88863-121">id</span></span>|<span data-ttu-id="88863-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88863-122">String</span></span>|<span data-ttu-id="88863-123">O identificador da política.</span><span class="sxs-lookup"><span data-stu-id="88863-123">The identifier of the policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88863-124">Relações</span><span class="sxs-lookup"><span data-stu-id="88863-124">Relationships</span></span>

|<span data-ttu-id="88863-125">Relação</span><span class="sxs-lookup"><span data-stu-id="88863-125">Relationship</span></span>|<span data-ttu-id="88863-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="88863-126">Type</span></span>|<span data-ttu-id="88863-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="88863-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88863-128">onSignupStart</span><span class="sxs-lookup"><span data-stu-id="88863-128">onSignupStart</span></span>|<span data-ttu-id="88863-129">coleção [authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="88863-129">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="88863-130">Uma lista de ações aplicáveis a serem executadas na inscrição.</span><span class="sxs-lookup"><span data-stu-id="88863-130">A list of applicable actions to be taken on sign-up.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88863-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88863-131">JSON representation</span></span>

<span data-ttu-id="88863-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88863-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```
