---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a2e41d9b17ca7acafa98dad65db5d2ff5ce30925
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572938"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="4014b-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="4014b-103">reportRoot resource type</span></span>

> <span data-ttu-id="4014b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4014b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4014b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4014b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4014b-106">O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="4014b-106">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="4014b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4014b-107">Methods</span></span>
|<span data-ttu-id="4014b-108">Método</span><span class="sxs-lookup"><span data-stu-id="4014b-108">Method</span></span>|<span data-ttu-id="4014b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4014b-109">Return Type</span></span>|<span data-ttu-id="4014b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4014b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4014b-111">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="4014b-111">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="4014b-112">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="4014b-112">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="4014b-113">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="4014b-113">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="4014b-114">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="4014b-114">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="4014b-115">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="4014b-115">**Device configuration**</span></span>|
|[<span data-ttu-id="4014b-116">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="4014b-116">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="4014b-117">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4014b-117">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="4014b-118">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="4014b-118">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="4014b-119">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4014b-119">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="4014b-120">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="4014b-120">**Troubleshooting**</span></span>|
|[<span data-ttu-id="4014b-121">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="4014b-121">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="4014b-122">relatório</span><span class="sxs-lookup"><span data-stu-id="4014b-122">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="4014b-123">Metadados para o relatório de detalhes de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="4014b-123">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="4014b-124">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="4014b-124">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="4014b-125">relatório</span><span class="sxs-lookup"><span data-stu-id="4014b-125">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="4014b-126">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="4014b-126">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="4014b-127">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="4014b-127">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="4014b-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4014b-128">Not yet documented</span></span>|
|[<span data-ttu-id="4014b-129">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="4014b-129">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="4014b-130">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="4014b-130">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="4014b-131">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="4014b-131">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="4014b-132">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4014b-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4014b-133">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4014b-133">Properties</span></span>
|<span data-ttu-id="4014b-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4014b-134">Property</span></span>|<span data-ttu-id="4014b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="4014b-135">Type</span></span>|<span data-ttu-id="4014b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="4014b-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4014b-137">id</span><span class="sxs-lookup"><span data-stu-id="4014b-137">id</span></span>|<span data-ttu-id="4014b-138">String</span><span class="sxs-lookup"><span data-stu-id="4014b-138">String</span></span>|<span data-ttu-id="4014b-139">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="4014b-139">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4014b-140">Relações</span><span class="sxs-lookup"><span data-stu-id="4014b-140">Relationships</span></span>
<span data-ttu-id="4014b-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4014b-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4014b-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4014b-142">JSON Representation</span></span>
<span data-ttu-id="4014b-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4014b-143">Here is a JSON representation of the resource.</span></span>
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



