---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: c975abfa3cb580d107967c7adaf66627bad2ad2e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938727"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="ce40a-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="ce40a-103">reportRoot resource type</span></span>

> <span data-ttu-id="ce40a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce40a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce40a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce40a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce40a-106">O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="ce40a-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="ce40a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ce40a-107">Methods</span></span>
|<span data-ttu-id="ce40a-108">Método</span><span class="sxs-lookup"><span data-stu-id="ce40a-108">Method</span></span>|<span data-ttu-id="ce40a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ce40a-109">Return Type</span></span>|<span data-ttu-id="ce40a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce40a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce40a-111">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="ce40a-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="ce40a-112">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="ce40a-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="ce40a-113">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="ce40a-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="ce40a-114">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="ce40a-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="ce40a-115">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="ce40a-115">**Device configuration**</span></span>|
|[<span data-ttu-id="ce40a-116">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="ce40a-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="ce40a-117">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ce40a-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="ce40a-118">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="ce40a-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="ce40a-119">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ce40a-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="ce40a-120">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="ce40a-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="ce40a-121">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="ce40a-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="ce40a-122">relatório</span><span class="sxs-lookup"><span data-stu-id="ce40a-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="ce40a-123">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="ce40a-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="ce40a-124">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="ce40a-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="ce40a-125">relatório</span><span class="sxs-lookup"><span data-stu-id="ce40a-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="ce40a-126">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="ce40a-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="ce40a-127">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="ce40a-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="ce40a-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ce40a-128">Not yet documented</span></span>|
|[<span data-ttu-id="ce40a-129">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="ce40a-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="ce40a-130">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="ce40a-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="ce40a-131">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="ce40a-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="ce40a-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ce40a-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ce40a-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce40a-133">Properties</span></span>
|<span data-ttu-id="ce40a-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce40a-134">Property</span></span>|<span data-ttu-id="ce40a-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce40a-135">Type</span></span>|<span data-ttu-id="ce40a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce40a-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce40a-137">id</span><span class="sxs-lookup"><span data-stu-id="ce40a-137">id</span></span>|<span data-ttu-id="ce40a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce40a-138">String</span></span>|<span data-ttu-id="ce40a-139">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="ce40a-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce40a-140">Relações</span><span class="sxs-lookup"><span data-stu-id="ce40a-140">Relationships</span></span>
<span data-ttu-id="ce40a-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce40a-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce40a-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce40a-142">JSON Representation</span></span>
<span data-ttu-id="ce40a-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce40a-143">Here is a JSON representation of the resource.</span></span>
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



