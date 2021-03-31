---
title: Tipo de recurso adminConsentRequestPolicy
description: Especifica a política pela qual as solicitações de consentimento podem ser criadas e gerenciadas para todo o locatário.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d7fadabdd8bc3581a2a32b70fad2b27c71c3b5c
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469513"
---
# <a name="adminconsentrequestpolicy-resource-type"></a><span data-ttu-id="fda6e-103">Tipo de recurso adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="fda6e-103">adminConsentRequestPolicy resource type</span></span>

<span data-ttu-id="fda6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fda6e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fda6e-105">Especifica a política pela qual as solicitações de consentimento são criadas e gerenciadas para todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="fda6e-105">Specifies the policy by which consent requests are created and managed for the entire tenant.</span></span> <span data-ttu-id="fda6e-106">Há um único **adminConsentRequestPolicy** por locatário.</span><span class="sxs-lookup"><span data-stu-id="fda6e-106">There is a single **adminConsentRequestPolicy** per tenant.</span></span>

<span data-ttu-id="fda6e-107">O **adminConsentRequestPolicy** fornece configurações adicionais ao criar uma solicitação de consentimento para controlar o comportamento do recurso ao iniciar uma solicitação de consentimento.</span><span class="sxs-lookup"><span data-stu-id="fda6e-107">The **adminConsentRequestPolicy** provides additional settings when creating a consent request, to control the feature behavior when starting a consent request.</span></span>

## <a name="methods"></a><span data-ttu-id="fda6e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="fda6e-108">Methods</span></span>

|<span data-ttu-id="fda6e-109">Método</span><span class="sxs-lookup"><span data-stu-id="fda6e-109">Method</span></span>|<span data-ttu-id="fda6e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fda6e-110">Return type</span></span>|<span data-ttu-id="fda6e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fda6e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fda6e-112">Obter adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="fda6e-112">Get adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-get.md)|[<span data-ttu-id="fda6e-113">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="fda6e-113">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="fda6e-114">Leia as propriedades e as relações de um [objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fda6e-114">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|
|[<span data-ttu-id="fda6e-115">Atualizar adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="fda6e-115">Update adminConsentRequestPolicy</span></span>](../api/adminconsentrequestpolicy-update.md)|[<span data-ttu-id="fda6e-116">adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="fda6e-116">adminConsentRequestPolicy</span></span>](../resources/adminconsentrequestpolicy.md)|<span data-ttu-id="fda6e-117">Atualize as propriedades de [um objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="fda6e-117">Update the properties of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fda6e-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fda6e-118">Properties</span></span>

|<span data-ttu-id="fda6e-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fda6e-119">Property</span></span>|<span data-ttu-id="fda6e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="fda6e-120">Type</span></span>|<span data-ttu-id="fda6e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fda6e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fda6e-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="fda6e-122">isEnabled</span></span>|<span data-ttu-id="fda6e-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="fda6e-123">Boolean</span></span>|<span data-ttu-id="fda6e-124">Especifica se o recurso de solicitação de consentimento do administrador está habilitado ou desabilitado.</span><span class="sxs-lookup"><span data-stu-id="fda6e-124">Specifies whether the admin consent request feature is enabled or disabled.</span></span> <span data-ttu-id="fda6e-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fda6e-125">Required.</span></span>|
|<span data-ttu-id="fda6e-126">notifyReviewers</span><span class="sxs-lookup"><span data-stu-id="fda6e-126">notifyReviewers</span></span>|<span data-ttu-id="fda6e-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="fda6e-127">Boolean</span></span>|<span data-ttu-id="fda6e-128">Especifica se os revisadores receberão notificações.</span><span class="sxs-lookup"><span data-stu-id="fda6e-128">Specifies whether reviewers will receive notifications.</span></span> <span data-ttu-id="fda6e-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fda6e-129">Required.</span></span>|
|<span data-ttu-id="fda6e-130">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="fda6e-130">remindersEnabled</span></span>|<span data-ttu-id="fda6e-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="fda6e-131">Boolean</span></span>|<span data-ttu-id="fda6e-132">Especifica se os revisadores receberão emails de lembrete.</span><span class="sxs-lookup"><span data-stu-id="fda6e-132">Specifies whether reviewers will receive reminder emails.</span></span> <span data-ttu-id="fda6e-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fda6e-133">Required.</span></span>|
|<span data-ttu-id="fda6e-134">requestDurationInDays</span><span class="sxs-lookup"><span data-stu-id="fda6e-134">requestDurationInDays</span></span>|<span data-ttu-id="fda6e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="fda6e-135">Int32</span></span>|<span data-ttu-id="fda6e-136">Especifica a duração em que a solicitação está ativa antes de expirar automaticamente se nenhuma decisão for aplicada.</span><span class="sxs-lookup"><span data-stu-id="fda6e-136">Specifies the duration the request is active before it automatically expires if no decision is applied.</span></span>|
|<span data-ttu-id="fda6e-137">revisadores</span><span class="sxs-lookup"><span data-stu-id="fda6e-137">reviewers</span></span>|<span data-ttu-id="fda6e-138">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="fda6e-138">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="fda6e-139">A lista de revisadores para o consentimento do administrador.</span><span class="sxs-lookup"><span data-stu-id="fda6e-139">The list of reviewers for the admin consent.</span></span> <span data-ttu-id="fda6e-140">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fda6e-140">Required.</span></span>|
|<span data-ttu-id="fda6e-141">versão</span><span class="sxs-lookup"><span data-stu-id="fda6e-141">version</span></span>|<span data-ttu-id="fda6e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fda6e-142">Int32</span></span>|<span data-ttu-id="fda6e-143">Especifica a versão dessa política.</span><span class="sxs-lookup"><span data-stu-id="fda6e-143">Specifies the version of this policy.</span></span> <span data-ttu-id="fda6e-144">Quando a política é atualizada, essa versão é atualizada.</span><span class="sxs-lookup"><span data-stu-id="fda6e-144">When the policy is updated, this version is updated.</span></span> <span data-ttu-id="fda6e-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fda6e-145">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fda6e-146">Relações</span><span class="sxs-lookup"><span data-stu-id="fda6e-146">Relationships</span></span>

<span data-ttu-id="fda6e-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fda6e-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fda6e-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fda6e-148">JSON representation</span></span>

<span data-ttu-id="fda6e-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fda6e-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "isEnabled": "Boolean",
  "version": "Integer",
  "notifyReviewers": "Boolean",
  "remindersEnabled": "Boolean",
  "requestDurationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```

