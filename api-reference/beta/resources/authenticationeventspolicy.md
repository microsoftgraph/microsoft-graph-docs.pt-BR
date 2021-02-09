---
title: Tipo de recurso authenticationEventsPolicy
description: Os eventos de autenticação são usados para invocar fluxos de usuário em pontos específicos no fluxo de autenticação.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4fe50176ebf49d79adc1db55c657bcf7fed8f096
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159945"
---
# <a name="authenticationeventspolicy-resource-type"></a><span data-ttu-id="fc549-103">Tipo de recurso authenticationEventsPolicy</span><span class="sxs-lookup"><span data-stu-id="fc549-103">authenticationEventsPolicy resource type</span></span>

<span data-ttu-id="fc549-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc549-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc549-105">Um recurso que especifica os eventos na experiência de autenticação, com cada evento definindo ainda mais os tipos disponíveis de ouvintes que podem ser criados para o evento.</span><span class="sxs-lookup"><span data-stu-id="fc549-105">A resource that specifies the events in the authentication experience, with each event further defining the available types of listeners that can be created for the event.</span></span> <span data-ttu-id="fc549-106">Os eventos são inerentes à experiência de autenticação; esse recurso não é configurável pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="fc549-106">Events are inherent to the authentication experience; this resource is not user configurable.</span></span>

## <a name="methods"></a><span data-ttu-id="fc549-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc549-107">Methods</span></span>

|<span data-ttu-id="fc549-108">Método</span><span class="sxs-lookup"><span data-stu-id="fc549-108">Method</span></span>|<span data-ttu-id="fc549-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc549-109">Return type</span></span>|<span data-ttu-id="fc549-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc549-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fc549-111">Listar ouvintes onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="fc549-111">List onSignUpStart listeners</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="fc549-112">[Coleção authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="fc549-112">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="fc549-113">Obter a coleção de recursos authenticationListener suportados pelo evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="fc549-113">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="fc549-114">Criar authenticationListener</span><span class="sxs-lookup"><span data-stu-id="fc549-114">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="fc549-115">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="fc549-115">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="fc549-116">Crie um novo objeto authenticationListener para o evento onSignupStart.</span><span class="sxs-lookup"><span data-stu-id="fc549-116">Create a new authenticationListener object for the onSignupStart event.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc549-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc549-117">Properties</span></span>

|<span data-ttu-id="fc549-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc549-118">Property</span></span>|<span data-ttu-id="fc549-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc549-119">Type</span></span>|<span data-ttu-id="fc549-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc549-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc549-121">id</span><span class="sxs-lookup"><span data-stu-id="fc549-121">id</span></span>|<span data-ttu-id="fc549-122">String</span><span class="sxs-lookup"><span data-stu-id="fc549-122">String</span></span>|<span data-ttu-id="fc549-123">O identificador da política.</span><span class="sxs-lookup"><span data-stu-id="fc549-123">The identifier of the policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc549-124">Relações</span><span class="sxs-lookup"><span data-stu-id="fc549-124">Relationships</span></span>

|<span data-ttu-id="fc549-125">Relação</span><span class="sxs-lookup"><span data-stu-id="fc549-125">Relationship</span></span>|<span data-ttu-id="fc549-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc549-126">Type</span></span>|<span data-ttu-id="fc549-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc549-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc549-128">onSignupStart</span><span class="sxs-lookup"><span data-stu-id="fc549-128">onSignupStart</span></span>|<span data-ttu-id="fc549-129">[Coleção authenticationListener](../resources/authenticationlistener.md)</span><span class="sxs-lookup"><span data-stu-id="fc549-129">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="fc549-130">Uma lista de ações aplicáveis a serem tomadas na assinatura.</span><span class="sxs-lookup"><span data-stu-id="fc549-130">A list of applicable actions to be taken on sign-up.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc549-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc549-131">JSON representation</span></span>

<span data-ttu-id="fc549-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc549-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```
