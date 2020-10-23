---
title: tipo de recurso securityBaselineStateSummary
description: O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2ee720f2fa5fa456431ec9f9329c72868503959
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690627"
---
# <a name="securitybaselinestatesummary-resource-type"></a><span data-ttu-id="57148-103">tipo de recurso securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="57148-103">securityBaselineStateSummary resource type</span></span>

<span data-ttu-id="57148-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57148-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57148-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57148-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57148-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57148-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57148-107">O resumo do estado de conformidade da linha de base de segurança para a linha de base de segurança da conta.</span><span class="sxs-lookup"><span data-stu-id="57148-107">The security baseline compliance state summary for the security baseline of the account.</span></span>

## <a name="methods"></a><span data-ttu-id="57148-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="57148-108">Methods</span></span>
|<span data-ttu-id="57148-109">Método</span><span class="sxs-lookup"><span data-stu-id="57148-109">Method</span></span>|<span data-ttu-id="57148-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="57148-110">Return Type</span></span>|<span data-ttu-id="57148-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="57148-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57148-112">Obter securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="57148-112">Get securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[<span data-ttu-id="57148-113">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="57148-113">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="57148-114">Leia as propriedades e as relações do objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="57148-114">Read properties and relationships of the [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|
|[<span data-ttu-id="57148-115">Atualizar securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="57148-115">Update securityBaselineStateSummary</span></span>](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[<span data-ttu-id="57148-116">securityBaselineStateSummary</span><span class="sxs-lookup"><span data-stu-id="57148-116">securityBaselineStateSummary</span></span>](../resources/intune-deviceintent-securitybaselinestatesummary.md)|<span data-ttu-id="57148-117">Atualiza as propriedades de um objeto [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="57148-117">Update the properties of a [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="57148-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57148-118">Properties</span></span>
|<span data-ttu-id="57148-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57148-119">Property</span></span>|<span data-ttu-id="57148-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="57148-120">Type</span></span>|<span data-ttu-id="57148-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="57148-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57148-122">id</span><span class="sxs-lookup"><span data-stu-id="57148-122">id</span></span>|<span data-ttu-id="57148-123">String</span><span class="sxs-lookup"><span data-stu-id="57148-123">String</span></span>|<span data-ttu-id="57148-124">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="57148-124">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="57148-125">secureCount</span><span class="sxs-lookup"><span data-stu-id="57148-125">secureCount</span></span>|<span data-ttu-id="57148-126">Int32</span><span class="sxs-lookup"><span data-stu-id="57148-126">Int32</span></span>|<span data-ttu-id="57148-127">Número de dispositivos seguros</span><span class="sxs-lookup"><span data-stu-id="57148-127">Number of secure devices</span></span>|
|<span data-ttu-id="57148-128">notSecureCount</span><span class="sxs-lookup"><span data-stu-id="57148-128">notSecureCount</span></span>|<span data-ttu-id="57148-129">Int32</span><span class="sxs-lookup"><span data-stu-id="57148-129">Int32</span></span>|<span data-ttu-id="57148-130">Número de dispositivos não seguros</span><span class="sxs-lookup"><span data-stu-id="57148-130">Number of not secure devices</span></span>|
|<span data-ttu-id="57148-131">unknownCount</span><span class="sxs-lookup"><span data-stu-id="57148-131">unknownCount</span></span>|<span data-ttu-id="57148-132">Int32</span><span class="sxs-lookup"><span data-stu-id="57148-132">Int32</span></span>|<span data-ttu-id="57148-133">Número de dispositivos desconhecidos</span><span class="sxs-lookup"><span data-stu-id="57148-133">Number of unknown devices</span></span>|
|<span data-ttu-id="57148-134">errorCount</span><span class="sxs-lookup"><span data-stu-id="57148-134">errorCount</span></span>|<span data-ttu-id="57148-135">Int32</span><span class="sxs-lookup"><span data-stu-id="57148-135">Int32</span></span>|<span data-ttu-id="57148-136">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="57148-136">Number of error devices</span></span>|
|<span data-ttu-id="57148-137">conflictCount</span><span class="sxs-lookup"><span data-stu-id="57148-137">conflictCount</span></span>|<span data-ttu-id="57148-138">Int32</span><span class="sxs-lookup"><span data-stu-id="57148-138">Int32</span></span>|<span data-ttu-id="57148-139">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="57148-139">Number of conflict devices</span></span>|
|<span data-ttu-id="57148-140">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="57148-140">notApplicableCount</span></span>|<span data-ttu-id="57148-141">Int32</span><span class="sxs-lookup"><span data-stu-id="57148-141">Int32</span></span>|<span data-ttu-id="57148-142">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="57148-142">Number of not applicable devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="57148-143">Relações</span><span class="sxs-lookup"><span data-stu-id="57148-143">Relationships</span></span>
<span data-ttu-id="57148-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57148-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57148-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57148-145">JSON Representation</span></span>
<span data-ttu-id="57148-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57148-146">Here is a JSON representation of the resource.</span></span>
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





