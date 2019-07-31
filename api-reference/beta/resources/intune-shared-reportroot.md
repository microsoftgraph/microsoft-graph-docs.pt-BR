---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 474ac908edee316a63c3610782cc4b8dcce070f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967362"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="d6ba8-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="d6ba8-103">reportRoot resource type</span></span>

> <span data-ttu-id="d6ba8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6ba8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6ba8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6ba8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6ba8-106">O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="d6ba8-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="d6ba8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d6ba8-107">Methods</span></span>
|<span data-ttu-id="d6ba8-108">Método</span><span class="sxs-lookup"><span data-stu-id="d6ba8-108">Method</span></span>|<span data-ttu-id="d6ba8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d6ba8-109">Return Type</span></span>|<span data-ttu-id="d6ba8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ba8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6ba8-111">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="d6ba8-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="d6ba8-112">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d6ba8-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="d6ba8-113">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="d6ba8-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="d6ba8-114">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d6ba8-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="d6ba8-115">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d6ba8-115">**Device configuration**</span></span>|
|[<span data-ttu-id="d6ba8-116">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="d6ba8-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="d6ba8-117">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d6ba8-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="d6ba8-118">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="d6ba8-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="d6ba8-119">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d6ba8-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="d6ba8-120">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="d6ba8-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="d6ba8-121">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="d6ba8-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="d6ba8-122">relatório</span><span class="sxs-lookup"><span data-stu-id="d6ba8-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="d6ba8-123">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="d6ba8-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="d6ba8-124">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="d6ba8-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="d6ba8-125">relatório</span><span class="sxs-lookup"><span data-stu-id="d6ba8-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="d6ba8-126">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="d6ba8-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="d6ba8-127">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="d6ba8-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="d6ba8-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ba8-128">Not yet documented</span></span>|
|[<span data-ttu-id="d6ba8-129">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="d6ba8-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="d6ba8-130">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="d6ba8-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="d6ba8-131">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="d6ba8-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="d6ba8-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d6ba8-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d6ba8-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6ba8-133">Properties</span></span>
|<span data-ttu-id="d6ba8-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6ba8-134">Property</span></span>|<span data-ttu-id="d6ba8-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6ba8-135">Type</span></span>|<span data-ttu-id="d6ba8-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ba8-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6ba8-137">id</span><span class="sxs-lookup"><span data-stu-id="d6ba8-137">id</span></span>|<span data-ttu-id="d6ba8-138">String</span><span class="sxs-lookup"><span data-stu-id="d6ba8-138">String</span></span>|<span data-ttu-id="d6ba8-139">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="d6ba8-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6ba8-140">Relações</span><span class="sxs-lookup"><span data-stu-id="d6ba8-140">Relationships</span></span>
<span data-ttu-id="d6ba8-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6ba8-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6ba8-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6ba8-142">JSON Representation</span></span>
<span data-ttu-id="d6ba8-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6ba8-143">Here is a JSON representation of the resource.</span></span>
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



