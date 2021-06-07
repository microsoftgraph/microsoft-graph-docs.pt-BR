---
title: Tipo de recurso officeConfiguration
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20e86afa8d0d5fddf5b87a6c6667e2e16baa391a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752829"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="2735b-103">Tipo de recurso officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2735b-103">officeConfiguration resource type</span></span>

<span data-ttu-id="2735b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2735b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2735b-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2735b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2735b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2735b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2735b-107">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2735b-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="2735b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2735b-108">Methods</span></span>
|<span data-ttu-id="2735b-109">Método</span><span class="sxs-lookup"><span data-stu-id="2735b-109">Method</span></span>|<span data-ttu-id="2735b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2735b-110">Return Type</span></span>|<span data-ttu-id="2735b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2735b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2735b-112">Obter officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2735b-112">Get officeConfiguration</span></span>|[<span data-ttu-id="2735b-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2735b-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="2735b-114">Leia propriedades e relações do [objeto officeConfiguration.](../resources/intune-cirrus-officeconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2735b-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="2735b-115">Atualizar officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2735b-115">Update officeConfiguration</span></span>|[<span data-ttu-id="2735b-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="2735b-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="2735b-117">Atualize as propriedades de um [objeto officeConfiguration.](../resources/intune-cirrus-officeconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2735b-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2735b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2735b-118">Properties</span></span>
|<span data-ttu-id="2735b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2735b-119">Property</span></span>|<span data-ttu-id="2735b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2735b-120">Type</span></span>|<span data-ttu-id="2735b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2735b-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2735b-122">id</span><span class="sxs-lookup"><span data-stu-id="2735b-122">id</span></span>|<span data-ttu-id="2735b-123">String</span><span class="sxs-lookup"><span data-stu-id="2735b-123">String</span></span>|<span data-ttu-id="2735b-124">ID da configuração do office.</span><span class="sxs-lookup"><span data-stu-id="2735b-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="2735b-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="2735b-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="2735b-126">[Coleção officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="2735b-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="2735b-127">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="2735b-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="2735b-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="2735b-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="2735b-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="2735b-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="2735b-130">Entidade que descreve as estatuetas de check-in do locatário</span><span class="sxs-lookup"><span data-stu-id="2735b-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="2735b-131">Relações</span><span class="sxs-lookup"><span data-stu-id="2735b-131">Relationships</span></span>
|<span data-ttu-id="2735b-132">Relação</span><span class="sxs-lookup"><span data-stu-id="2735b-132">Relationship</span></span>|<span data-ttu-id="2735b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="2735b-133">Type</span></span>|<span data-ttu-id="2735b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2735b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2735b-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="2735b-135">clientConfigurations</span></span>|<span data-ttu-id="2735b-136">[Coleção officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2735b-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="2735b-137">Lista de configuração do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="2735b-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2735b-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2735b-138">JSON Representation</span></span>
<span data-ttu-id="2735b-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2735b-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```




