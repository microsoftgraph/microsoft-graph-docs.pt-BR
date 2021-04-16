---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30b84ec908eea116442284d6c20e2b56be68ea3c
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863643"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="d1a04-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="d1a04-103">reportRoot resource type</span></span>

<span data-ttu-id="d1a04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1a04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1a04-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1a04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1a04-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1a04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1a04-107">O recurso que representa uma instância de um dispositivo ou relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="d1a04-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="d1a04-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d1a04-108">Methods</span></span>
|<span data-ttu-id="d1a04-109">Método</span><span class="sxs-lookup"><span data-stu-id="d1a04-109">Method</span></span>|<span data-ttu-id="d1a04-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d1a04-110">Return Type</span></span>|<span data-ttu-id="d1a04-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1a04-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d1a04-112">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="d1a04-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="d1a04-113">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d1a04-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="d1a04-114">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="d1a04-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="d1a04-115">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="d1a04-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="d1a04-116">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="d1a04-116">**Device configuration**</span></span>|
|[<span data-ttu-id="d1a04-117">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="d1a04-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="d1a04-118">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d1a04-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="d1a04-119">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="d1a04-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="d1a04-120">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d1a04-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="d1a04-121">**Solução de Problemas**</span><span class="sxs-lookup"><span data-stu-id="d1a04-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="d1a04-122">Função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="d1a04-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="d1a04-123">relatório</span><span class="sxs-lookup"><span data-stu-id="d1a04-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="d1a04-124">Relatório de detalhes de abandono de registro de metadados</span><span class="sxs-lookup"><span data-stu-id="d1a04-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="d1a04-125">Função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="d1a04-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="d1a04-126">relatório</span><span class="sxs-lookup"><span data-stu-id="d1a04-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="d1a04-127">Metadados para relatório de resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="d1a04-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="d1a04-128">Função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="d1a04-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="d1a04-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d1a04-129">Not yet documented</span></span>|
|[<span data-ttu-id="d1a04-130">Função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="d1a04-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="d1a04-131">Metadados para o relatório de tendências de falha de registro</span><span class="sxs-lookup"><span data-stu-id="d1a04-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="d1a04-132">Função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="d1a04-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="d1a04-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d1a04-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d1a04-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1a04-134">Properties</span></span>
|<span data-ttu-id="d1a04-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1a04-135">Property</span></span>|<span data-ttu-id="d1a04-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1a04-136">Type</span></span>|<span data-ttu-id="d1a04-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1a04-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1a04-138">id</span><span class="sxs-lookup"><span data-stu-id="d1a04-138">id</span></span>|<span data-ttu-id="d1a04-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1a04-139">String</span></span>|<span data-ttu-id="d1a04-140">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="d1a04-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1a04-141">Relações</span><span class="sxs-lookup"><span data-stu-id="d1a04-141">Relationships</span></span>
<span data-ttu-id="d1a04-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1a04-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1a04-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1a04-143">JSON Representation</span></span>
<span data-ttu-id="d1a04-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1a04-144">Here is a JSON representation of the resource.</span></span>
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




