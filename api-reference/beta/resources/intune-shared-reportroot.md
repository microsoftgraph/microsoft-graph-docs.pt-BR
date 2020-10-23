---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28d030eaf52f1656d4ba7da91c7cb3f6371958e3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726248"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="ffe70-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="ffe70-103">reportRoot resource type</span></span>

<span data-ttu-id="ffe70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffe70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffe70-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ffe70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffe70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ffe70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffe70-107">O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="ffe70-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="ffe70-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ffe70-108">Methods</span></span>
|<span data-ttu-id="ffe70-109">Método</span><span class="sxs-lookup"><span data-stu-id="ffe70-109">Method</span></span>|<span data-ttu-id="ffe70-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ffe70-110">Return Type</span></span>|<span data-ttu-id="ffe70-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffe70-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ffe70-112">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="ffe70-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="ffe70-113">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="ffe70-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="ffe70-114">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="ffe70-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="ffe70-115">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="ffe70-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="ffe70-116">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ffe70-116">**Device configuration**</span></span>|
|[<span data-ttu-id="ffe70-117">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="ffe70-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="ffe70-118">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ffe70-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="ffe70-119">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="ffe70-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="ffe70-120">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ffe70-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="ffe70-121">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ffe70-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="ffe70-122">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="ffe70-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="ffe70-123">relatório</span><span class="sxs-lookup"><span data-stu-id="ffe70-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="ffe70-124">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="ffe70-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="ffe70-125">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="ffe70-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="ffe70-126">relatório</span><span class="sxs-lookup"><span data-stu-id="ffe70-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="ffe70-127">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="ffe70-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="ffe70-128">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="ffe70-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="ffe70-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ffe70-129">Not yet documented</span></span>|
|[<span data-ttu-id="ffe70-130">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="ffe70-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="ffe70-131">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="ffe70-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="ffe70-132">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="ffe70-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="ffe70-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ffe70-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ffe70-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffe70-134">Properties</span></span>
|<span data-ttu-id="ffe70-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffe70-135">Property</span></span>|<span data-ttu-id="ffe70-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffe70-136">Type</span></span>|<span data-ttu-id="ffe70-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffe70-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe70-138">id</span><span class="sxs-lookup"><span data-stu-id="ffe70-138">id</span></span>|<span data-ttu-id="ffe70-139">String</span><span class="sxs-lookup"><span data-stu-id="ffe70-139">String</span></span>|<span data-ttu-id="ffe70-140">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="ffe70-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ffe70-141">Relações</span><span class="sxs-lookup"><span data-stu-id="ffe70-141">Relationships</span></span>
<span data-ttu-id="ffe70-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ffe70-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ffe70-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffe70-143">JSON Representation</span></span>
<span data-ttu-id="ffe70-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ffe70-144">Here is a JSON representation of the resource.</span></span>
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





