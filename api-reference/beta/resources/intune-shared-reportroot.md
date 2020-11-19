---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f986820ddacfc84c6cbea2233c6beec7f24946dd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271713"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="198f6-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="198f6-103">reportRoot resource type</span></span>

<span data-ttu-id="198f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="198f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="198f6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="198f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="198f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="198f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="198f6-107">O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="198f6-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="198f6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="198f6-108">Methods</span></span>
|<span data-ttu-id="198f6-109">Método</span><span class="sxs-lookup"><span data-stu-id="198f6-109">Method</span></span>|<span data-ttu-id="198f6-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="198f6-110">Return Type</span></span>|<span data-ttu-id="198f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="198f6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="198f6-112">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="198f6-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="198f6-113">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="198f6-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="198f6-114">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="198f6-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="198f6-115">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="198f6-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="198f6-116">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="198f6-116">**Device configuration**</span></span>|
|[<span data-ttu-id="198f6-117">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="198f6-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="198f6-118">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="198f6-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="198f6-119">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="198f6-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="198f6-120">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="198f6-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="198f6-121">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="198f6-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="198f6-122">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="198f6-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="198f6-123">relatório</span><span class="sxs-lookup"><span data-stu-id="198f6-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="198f6-124">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="198f6-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="198f6-125">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="198f6-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="198f6-126">relatório</span><span class="sxs-lookup"><span data-stu-id="198f6-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="198f6-127">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="198f6-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="198f6-128">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="198f6-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="198f6-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="198f6-129">Not yet documented</span></span>|
|[<span data-ttu-id="198f6-130">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="198f6-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="198f6-131">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="198f6-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="198f6-132">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="198f6-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="198f6-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="198f6-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="198f6-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="198f6-134">Properties</span></span>
|<span data-ttu-id="198f6-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="198f6-135">Property</span></span>|<span data-ttu-id="198f6-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="198f6-136">Type</span></span>|<span data-ttu-id="198f6-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="198f6-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="198f6-138">id</span><span class="sxs-lookup"><span data-stu-id="198f6-138">id</span></span>|<span data-ttu-id="198f6-139">String</span><span class="sxs-lookup"><span data-stu-id="198f6-139">String</span></span>|<span data-ttu-id="198f6-140">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="198f6-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="198f6-141">Relações</span><span class="sxs-lookup"><span data-stu-id="198f6-141">Relationships</span></span>
<span data-ttu-id="198f6-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="198f6-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="198f6-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="198f6-143">JSON Representation</span></span>
<span data-ttu-id="198f6-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="198f6-144">Here is a JSON representation of the resource.</span></span>
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




