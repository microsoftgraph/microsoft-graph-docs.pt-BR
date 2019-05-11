---
title: tipo de recurso officeConfiguration
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 7dfa6ead3de28daa0a5e3f4269578028dbc6b766
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949273"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="a105d-103">tipo de recurso officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a105d-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="a105d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a105d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a105d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a105d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a105d-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a105d-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="a105d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a105d-107">Methods</span></span>
|<span data-ttu-id="a105d-108">Método</span><span class="sxs-lookup"><span data-stu-id="a105d-108">Method</span></span>|<span data-ttu-id="a105d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a105d-109">Return Type</span></span>|<span data-ttu-id="a105d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a105d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a105d-111">Obter officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a105d-111">Get officeConfiguration</span></span>|[<span data-ttu-id="a105d-112">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a105d-112">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="a105d-113">Leia as propriedades e as relações do objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a105d-113">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="a105d-114">Atualizar officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a105d-114">Update officeConfiguration</span></span>|[<span data-ttu-id="a105d-115">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a105d-115">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="a105d-116">Atualiza as propriedades de um objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a105d-116">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a105d-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a105d-117">Properties</span></span>
|<span data-ttu-id="a105d-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a105d-118">Property</span></span>|<span data-ttu-id="a105d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="a105d-119">Type</span></span>|<span data-ttu-id="a105d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a105d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a105d-121">id</span><span class="sxs-lookup"><span data-stu-id="a105d-121">id</span></span>|<span data-ttu-id="a105d-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a105d-122">String</span></span>|<span data-ttu-id="a105d-123">ID da configuração do Office.</span><span class="sxs-lookup"><span data-stu-id="a105d-123">Id of the office configuration.</span></span>|
|<span data-ttu-id="a105d-124">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="a105d-124">tenantCheckinStatuses</span></span>|<span data-ttu-id="a105d-125">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="a105d-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="a105d-126">Lista de status de check-in do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="a105d-126">List of office Client check-in status.</span></span>|
|<span data-ttu-id="a105d-127">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="a105d-127">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="a105d-128">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="a105d-128">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="a105d-129">Entidade que descreve o check-in do locatário Statues</span><span class="sxs-lookup"><span data-stu-id="a105d-129">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="a105d-130">Relações</span><span class="sxs-lookup"><span data-stu-id="a105d-130">Relationships</span></span>
|<span data-ttu-id="a105d-131">Relação</span><span class="sxs-lookup"><span data-stu-id="a105d-131">Relationship</span></span>|<span data-ttu-id="a105d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a105d-132">Type</span></span>|<span data-ttu-id="a105d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a105d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a105d-134">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="a105d-134">clientConfigurations</span></span>|<span data-ttu-id="a105d-135">coleção [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a105d-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="a105d-136">Lista de configurações do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="a105d-136">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a105d-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a105d-137">JSON Representation</span></span>
<span data-ttu-id="a105d-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a105d-138">Here is a JSON representation of the resource.</span></span>
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



