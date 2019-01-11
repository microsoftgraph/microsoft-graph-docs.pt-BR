---
title: Tipo de recurso reportRoot
description: O recurso que representa uma instância de um dispositivo ou o relatório de solução de problemas, dependendo do contexto.
localization_priority: Normal
ms.openlocfilehash: 8a2c1cbc666698eea7f466c32bae6c404264f545
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809643"
---
# <a name="reportroot-resource-type"></a><span data-ttu-id="3a544-103">Tipo de recurso reportRoot</span><span class="sxs-lookup"><span data-stu-id="3a544-103">reportRoot resource type</span></span>

> <span data-ttu-id="3a544-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a544-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a544-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a544-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a544-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3a544-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a544-107">O recurso que representa uma instância de um dispositivo ou o relatório de solução de problemas, dependendo do contexto.</span><span class="sxs-lookup"><span data-stu-id="3a544-107">The resource that represents an instance of a device or troubleshooting report, depending on context.</span></span>

## <a name="methods"></a><span data-ttu-id="3a544-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3a544-108">Methods</span></span>
|<span data-ttu-id="3a544-109">Método</span><span class="sxs-lookup"><span data-stu-id="3a544-109">Method</span></span>|<span data-ttu-id="3a544-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3a544-110">Return Type</span></span>|<span data-ttu-id="3a544-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a544-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3a544-112">Obter reportRoot</span><span class="sxs-lookup"><span data-stu-id="3a544-112">Get reportRoot</span></span>](../api/intune-shared-reportroot-get.md)|<span data-ttu-id="3a544-113">Ler propriedades e relações de objetos de [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="3a544-113">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|[<span data-ttu-id="3a544-114">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="3a544-114">Update reportRoot</span></span>](../api/intune-shared-reportroot-update.md)|<span data-ttu-id="3a544-115">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="3a544-115">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>|
|<span data-ttu-id="3a544-116">**Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="3a544-116">**Device configuration**</span></span>|
|[<span data-ttu-id="3a544-117">Função deviceConfigurationUserActivity</span><span class="sxs-lookup"><span data-stu-id="3a544-117">deviceConfigurationUserActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationuseractivity.md)|<span data-ttu-id="3a544-118">Metadados para o Relatório de atividades do usuário de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3a544-118">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="3a544-119">função deviceConfigurationDeviceActivity</span><span class="sxs-lookup"><span data-stu-id="3a544-119">deviceConfigurationDeviceActivity function</span></span>](../api/intune-shared-reportroot-deviceconfigurationdeviceactivity.md)|<span data-ttu-id="3a544-120">Metadados para o relatório de atividade do dispositivo de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3a544-120">Metadata for the device configuration device activity report</span></span>|
|<span data-ttu-id="3a544-121">**Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="3a544-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="3a544-122">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="3a544-122">managedDeviceEnrollmentAbandonmentDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentdetails.md)|[<span data-ttu-id="3a544-123">relatório</span><span class="sxs-lookup"><span data-stu-id="3a544-123">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="3a544-124">Metadados para o relatório de detalhes de abandono de inscrição</span><span class="sxs-lookup"><span data-stu-id="3a544-124">Metadata for Enrollment abandonment details report</span></span>|
|[<span data-ttu-id="3a544-125">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="3a544-125">managedDeviceEnrollmentAbandonmentSummary function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentabandonmentsummary.md)|[<span data-ttu-id="3a544-126">relatório</span><span class="sxs-lookup"><span data-stu-id="3a544-126">report</span></span>](../resources/intune-shared-report.md)|<span data-ttu-id="3a544-127">Metadados para o relatório de resumo de abandono de inscrição</span><span class="sxs-lookup"><span data-stu-id="3a544-127">Metadata for Enrollment abandonment summary report</span></span>|
|[<span data-ttu-id="3a544-128">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="3a544-128">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails.md)|<span data-ttu-id="3a544-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3a544-129">Not yet documented</span></span>|
|[<span data-ttu-id="3a544-130">função managedDeviceEnrollmentFailureTrends</span><span class="sxs-lookup"><span data-stu-id="3a544-130">managedDeviceEnrollmentFailureTrends function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmentfailuretrends.md)|<span data-ttu-id="3a544-131">Metadados para o relatório de tendências de falha de inscrição</span><span class="sxs-lookup"><span data-stu-id="3a544-131">Metadata for the enrollment failure trends report</span></span>|
|[<span data-ttu-id="3a544-132">função managedDeviceEnrollmentTopFailures</span><span class="sxs-lookup"><span data-stu-id="3a544-132">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune-shared-reportroot-manageddeviceenrollmenttopfailures.md)|<span data-ttu-id="3a544-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3a544-133">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3a544-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a544-134">Properties</span></span>
|<span data-ttu-id="3a544-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a544-135">Property</span></span>|<span data-ttu-id="3a544-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a544-136">Type</span></span>|<span data-ttu-id="3a544-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a544-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a544-138">id</span><span class="sxs-lookup"><span data-stu-id="3a544-138">id</span></span>|<span data-ttu-id="3a544-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a544-139">String</span></span>|<span data-ttu-id="3a544-140">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="3a544-140">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a544-141">Relações</span><span class="sxs-lookup"><span data-stu-id="3a544-141">Relationships</span></span>
<span data-ttu-id="3a544-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a544-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a544-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a544-143">JSON Representation</span></span>
<span data-ttu-id="3a544-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a544-144">Here is a JSON representation of the resource.</span></span>
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



