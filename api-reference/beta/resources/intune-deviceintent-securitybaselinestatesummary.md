---
title: tipo de recurso securityBaselineStateSummary
description: O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c7c1cf31ddca02348eed55b9dc19dd5420b016e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943267"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="7ee0c-103">tipo de recurso securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="7ee0c-103">securityBaselineStateSummary resource type</span></span>

> <span data-ttu-id="7ee0c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ee0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ee0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ee0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ee0c-106">O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.</span><span class="sxs-lookup"><span data-stu-id="7ee0c-106">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="7ee0c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7ee0c-107">Methods</span></span>
|<span data-ttu-id="7ee0c-108">Método</span><span class="sxs-lookup"><span data-stu-id="7ee0c-108">Method</span></span>|<span data-ttu-id="7ee0c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7ee0c-109">Return Type</span></span>|<span data-ttu-id="7ee0c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ee0c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7ee0c-111">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="7ee0c-111">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="7ee0c-112">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="7ee0c-112">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="7ee0c-113">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7ee0c-113">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="7ee0c-114">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="7ee0c-114">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="7ee0c-115">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="7ee0c-115">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="7ee0c-116">Atualiza as propriedades de um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="7ee0c-116">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7ee0c-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ee0c-117">Properties</span></span>
|<span data-ttu-id="7ee0c-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ee0c-118">Property</span></span>|<span data-ttu-id="7ee0c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ee0c-119">Type</span></span>|<span data-ttu-id="7ee0c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ee0c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ee0c-121">id</span><span class="sxs-lookup"><span data-stu-id="7ee0c-121">id</span></span>|<span data-ttu-id="7ee0c-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ee0c-122">String</span></span>|<span data-ttu-id="7ee0c-123">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="7ee0c-123">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7ee0c-124">secureCount</span><span class="sxs-lookup"><span data-stu-id="7ee0c-124">secureCount</span></span>|<span data-ttu-id="7ee0c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee0c-125">Int32</span></span>|<span data-ttu-id="7ee0c-126">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="7ee0c-126">Number of secure devices</span></span>|
|<span data-ttu-id="7ee0c-127">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="7ee0c-127">notSecureCount</span></span>|<span data-ttu-id="7ee0c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee0c-128">Int32</span></span>|<span data-ttu-id="7ee0c-129">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="7ee0c-129">Number of not secure devices</span></span>|
|<span data-ttu-id="7ee0c-130">unknownCount</span><span class="sxs-lookup"><span data-stu-id="7ee0c-130">unknownCount</span></span>|<span data-ttu-id="7ee0c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee0c-131">Int32</span></span>|<span data-ttu-id="7ee0c-132">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="7ee0c-132">Number of unknown devices</span></span>|
|<span data-ttu-id="7ee0c-133">errorCount</span><span class="sxs-lookup"><span data-stu-id="7ee0c-133">errorCount</span></span>|<span data-ttu-id="7ee0c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee0c-134">Int32</span></span>|<span data-ttu-id="7ee0c-135">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="7ee0c-135">Number of error devices</span></span>|
|<span data-ttu-id="7ee0c-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="7ee0c-136">conflictCount</span></span>|<span data-ttu-id="7ee0c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee0c-137">Int32</span></span>|<span data-ttu-id="7ee0c-138">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="7ee0c-138">Number of conflict devices</span></span>|
|<span data-ttu-id="7ee0c-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="7ee0c-139">notApplicableCount</span></span>|<span data-ttu-id="7ee0c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7ee0c-140">Int32</span></span>|<span data-ttu-id="7ee0c-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="7ee0c-141">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ee0c-142">Relações</span><span class="sxs-lookup"><span data-stu-id="7ee0c-142">Relationships</span></span>
<span data-ttu-id="7ee0c-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ee0c-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ee0c-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ee0c-144">JSON Representation</span></span>
<span data-ttu-id="7ee0c-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ee0c-145">Here is a JSON representation of the resource.</span></span>
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




