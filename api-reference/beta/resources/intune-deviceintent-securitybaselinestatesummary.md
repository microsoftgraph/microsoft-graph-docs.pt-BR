---
title: tipo de recurso securityBaselineStateSummary
description: O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 28a479ec175a939d65d4d11c963df575a28e59d1
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523956"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="d9681-103">tipo de recurso securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9681-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="d9681-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9681-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9681-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9681-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9681-106">O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.</span><span class="sxs-lookup"><span data-stu-id="d9681-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="d9681-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d9681-107">Methods</span></span>
|<span data-ttu-id="d9681-108">Método</span><span class="sxs-lookup"><span data-stu-id="d9681-108">Method</span></span>|<span data-ttu-id="d9681-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d9681-109">Return Type</span></span>|<span data-ttu-id="d9681-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9681-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9681-111">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9681-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="d9681-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9681-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="d9681-113">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d9681-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="d9681-114">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9681-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="d9681-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="d9681-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="d9681-116">Atualiza as propriedades de um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d9681-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9681-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9681-117">Properties</span></span>
|<span data-ttu-id="d9681-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9681-118">Property</span></span>|<span data-ttu-id="d9681-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9681-119">Type</span></span>|<span data-ttu-id="d9681-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9681-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9681-121">id</span><span class="sxs-lookup"><span data-stu-id="d9681-121">id</span></span>|<span data-ttu-id="d9681-122">String</span><span class="sxs-lookup"><span data-stu-id="d9681-122">String</span></span>|<span data-ttu-id="d9681-123">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9681-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d9681-124">secureCount</span><span class="sxs-lookup"><span data-stu-id="d9681-124">secureCount</span></span>|<span data-ttu-id="d9681-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d9681-125">Int32</span></span>|<span data-ttu-id="d9681-126">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="d9681-126">Number of secure devices</span></span>|
|<span data-ttu-id="d9681-127">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="d9681-127">notSecureCount</span></span>|<span data-ttu-id="d9681-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d9681-128">Int32</span></span>|<span data-ttu-id="d9681-129">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="d9681-129">Number of not secure devices</span></span>|
|<span data-ttu-id="d9681-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d9681-130">unknownCount</span></span>|<span data-ttu-id="d9681-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d9681-131">Int32</span></span>|<span data-ttu-id="d9681-132">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="d9681-132">Number of unknown devices</span></span>|
|<span data-ttu-id="d9681-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="d9681-133">errorCount</span></span>|<span data-ttu-id="d9681-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d9681-134">Int32</span></span>|<span data-ttu-id="d9681-135">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="d9681-135">Number of error devices</span></span>|
|<span data-ttu-id="d9681-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d9681-136">conflictCount</span></span>|<span data-ttu-id="d9681-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d9681-137">Int32</span></span>|<span data-ttu-id="d9681-138">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="d9681-138">Number of conflict devices</span></span>|
|<span data-ttu-id="d9681-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d9681-139">notApplicableCount</span></span>|<span data-ttu-id="d9681-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d9681-140">Int32</span></span>|<span data-ttu-id="d9681-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="d9681-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9681-142">Relações</span><span class="sxs-lookup"><span data-stu-id="d9681-142">Relationships</span></span>
<span data-ttu-id="d9681-143">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d9681-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9681-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9681-144">JSON Representation</span></span>
<span data-ttu-id="d9681-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9681-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```







