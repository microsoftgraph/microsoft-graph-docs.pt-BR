---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f11a2b0bb3260d834900955886ad477030fd3351
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473533"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="9e0c8-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="9e0c8-103">reportRoot resource type</span></span>

<span data-ttu-id="9e0c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e0c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e0c8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e0c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e0c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e0c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e0c8-107">O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="9e0c8-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="9e0c8-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e0c8-108">Methods</span></span>
|<span data-ttu-id="9e0c8-109">Método</span><span class="sxs-lookup"><span data-stu-id="9e0c8-109">Method</span></span>|<span data-ttu-id="9e0c8-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e0c8-110">Return Type</span></span>|<span data-ttu-id="9e0c8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e0c8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9e0c8-112">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="9e0c8-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="9e0c8-113">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="9e0c8-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="9e0c8-114">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="9e0c8-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="9e0c8-115">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="9e0c8-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="9e0c8-116">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="9e0c8-116">**Device configuration**</span></span>|
|[<span data-ttu-id="9e0c8-117">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="9e0c8-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="9e0c8-118">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9e0c8-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="9e0c8-119">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="9e0c8-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="9e0c8-120">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9e0c8-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="9e0c8-121">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="9e0c8-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="9e0c8-122">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="9e0c8-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="9e0c8-123">relatório</span><span class="sxs-lookup"><span data-stu-id="9e0c8-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="9e0c8-124">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="9e0c8-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="9e0c8-125">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="9e0c8-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="9e0c8-126">relatório</span><span class="sxs-lookup"><span data-stu-id="9e0c8-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="9e0c8-127">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="9e0c8-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="9e0c8-128">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="9e0c8-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="9e0c8-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9e0c8-129">Not yet documented</span></span>|
|[<span data-ttu-id="9e0c8-130">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="9e0c8-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="9e0c8-131">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="9e0c8-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="9e0c8-132">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="9e0c8-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="9e0c8-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9e0c8-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="9e0c8-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e0c8-134">Properties</span></span>
|<span data-ttu-id="9e0c8-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e0c8-135">Property</span></span>|<span data-ttu-id="9e0c8-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e0c8-136">Type</span></span>|<span data-ttu-id="9e0c8-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e0c8-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e0c8-138">id</span><span class="sxs-lookup"><span data-stu-id="9e0c8-138">id</span></span>|<span data-ttu-id="9e0c8-139">String</span><span class="sxs-lookup"><span data-stu-id="9e0c8-139">String</span></span>|<span data-ttu-id="9e0c8-140">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="9e0c8-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e0c8-141">Relações</span><span class="sxs-lookup"><span data-stu-id="9e0c8-141">Relationships</span></span>
<span data-ttu-id="9e0c8-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9e0c8-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e0c8-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e0c8-143">JSON Representation</span></span>
<span data-ttu-id="9e0c8-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e0c8-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



