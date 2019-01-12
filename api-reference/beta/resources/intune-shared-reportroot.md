---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou o relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: efb8950b9956901161c822df8b467b0182a4cc75
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959584"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="61773-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="61773-103">reportRoot resource type</span></span>

> <span data-ttu-id="61773-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="61773-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61773-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="61773-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61773-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61773-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61773-107">O recurso que representa uma instância de um dispositivo ou o relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="61773-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="61773-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="61773-108">Methods</span></span>
|<span data-ttu-id="61773-109">Método</span><span class="sxs-lookup"><span data-stu-id="61773-109">Method</span></span>|<span data-ttu-id="61773-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61773-110">Return Type</span></span>|<span data-ttu-id="61773-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61773-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="61773-112">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="61773-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="61773-113">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="61773-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="61773-114">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="61773-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="61773-115">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="61773-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="61773-116">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="61773-116">**Device configuration**</span></span>|
|[<span data-ttu-id="61773-117">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="61773-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="61773-118">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="61773-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="61773-119">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="61773-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="61773-120">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="61773-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="61773-121">**Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="61773-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="61773-122">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="61773-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="61773-123">relatório</span><span class="sxs-lookup"><span data-stu-id="61773-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="61773-124">Metadados para o relatório de detalhes de abandono de inscrição</span><span class="sxs-lookup"><span data-stu-id="61773-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="61773-125">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="61773-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="61773-126">relatório</span><span class="sxs-lookup"><span data-stu-id="61773-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="61773-127">Metadados para o relatório de resumo de abandono de inscrição</span><span class="sxs-lookup"><span data-stu-id="61773-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="61773-128">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="61773-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="61773-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61773-129">Not yet documented</span></span>|
|[<span data-ttu-id="61773-130">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="61773-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="61773-131">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="61773-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="61773-132">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="61773-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="61773-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="61773-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="61773-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61773-134">Properties</span></span>
|<span data-ttu-id="61773-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61773-135">Property</span></span>|<span data-ttu-id="61773-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="61773-136">Type</span></span>|<span data-ttu-id="61773-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="61773-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61773-138">id</span><span class="sxs-lookup"><span data-stu-id="61773-138">id</span></span>|<span data-ttu-id="61773-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61773-139">String</span></span>|<span data-ttu-id="61773-140">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="61773-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61773-141">Relações</span><span class="sxs-lookup"><span data-stu-id="61773-141">Relationships</span></span>
<span data-ttu-id="61773-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61773-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61773-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61773-143">JSON Representation</span></span>
<span data-ttu-id="61773-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61773-144">Here is a JSON representation of the resource.</span></span>
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



