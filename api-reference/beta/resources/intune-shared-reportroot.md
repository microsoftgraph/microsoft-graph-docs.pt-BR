---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou o relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 378f1758773bfcffda5d9039d3b60d4ac4bd5cc5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421330"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="0c85a-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="0c85a-103">reportRoot resource type</span></span>

> <span data-ttu-id="0c85a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c85a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c85a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c85a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c85a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0c85a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c85a-107">O recurso que representa uma instância de um dispositivo ou o relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="0c85a-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="0c85a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c85a-108">Methods</span></span>
|<span data-ttu-id="0c85a-109">Método</span><span class="sxs-lookup"><span data-stu-id="0c85a-109">Method</span></span>|<span data-ttu-id="0c85a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0c85a-110">Return Type</span></span>|<span data-ttu-id="0c85a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c85a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c85a-112">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="0c85a-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="0c85a-113">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="0c85a-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="0c85a-114">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="0c85a-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="0c85a-115">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="0c85a-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="0c85a-116">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="0c85a-116">**Device configuration**</span></span>|
|[<span data-ttu-id="0c85a-117">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="0c85a-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="0c85a-118">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0c85a-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="0c85a-119">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="0c85a-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="0c85a-120">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0c85a-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="0c85a-121">**Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="0c85a-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="0c85a-122">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="0c85a-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="0c85a-123">relatório</span><span class="sxs-lookup"><span data-stu-id="0c85a-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="0c85a-124">Metadados para o relatório de detalhes de abandono de inscrição</span><span class="sxs-lookup"><span data-stu-id="0c85a-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="0c85a-125">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="0c85a-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="0c85a-126">relatório</span><span class="sxs-lookup"><span data-stu-id="0c85a-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="0c85a-127">Metadados para o relatório de resumo de abandono de inscrição</span><span class="sxs-lookup"><span data-stu-id="0c85a-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="0c85a-128">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="0c85a-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="0c85a-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c85a-129">Not yet documented</span></span>|
|[<span data-ttu-id="0c85a-130">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="0c85a-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="0c85a-131">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="0c85a-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="0c85a-132">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="0c85a-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="0c85a-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c85a-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0c85a-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c85a-134">Properties</span></span>
|<span data-ttu-id="0c85a-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c85a-135">Property</span></span>|<span data-ttu-id="0c85a-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c85a-136">Type</span></span>|<span data-ttu-id="0c85a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c85a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c85a-138">id</span><span class="sxs-lookup"><span data-stu-id="0c85a-138">id</span></span>|<span data-ttu-id="0c85a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c85a-139">String</span></span>|<span data-ttu-id="0c85a-140">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="0c85a-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c85a-141">Relações</span><span class="sxs-lookup"><span data-stu-id="0c85a-141">Relationships</span></span>
<span data-ttu-id="0c85a-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c85a-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c85a-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c85a-143">JSON Representation</span></span>
<span data-ttu-id="0c85a-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c85a-144">Here is a JSON representation of the resource.</span></span>
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



