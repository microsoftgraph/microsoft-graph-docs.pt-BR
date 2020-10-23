---
title: tipo de recurso officeConfiguration
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 276a9bd60e988d0bb961ef849c8ce57d8eb9bb47
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723950"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="b25c9-103">tipo de recurso officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b25c9-103">officeConfiguration resource type</span></span>

<span data-ttu-id="b25c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b25c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b25c9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b25c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b25c9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b25c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b25c9-107">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="b25c9-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="b25c9-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b25c9-108">Methods</span></span>
|<span data-ttu-id="b25c9-109">Método</span><span class="sxs-lookup"><span data-stu-id="b25c9-109">Method</span></span>|<span data-ttu-id="b25c9-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b25c9-110">Return Type</span></span>|<span data-ttu-id="b25c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b25c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b25c9-112">Obter officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b25c9-112">Get officeConfiguration</span></span>|[<span data-ttu-id="b25c9-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b25c9-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="b25c9-114">Leia as propriedades e as relações do objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b25c9-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="b25c9-115">Atualizar officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b25c9-115">Update officeConfiguration</span></span>|[<span data-ttu-id="b25c9-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="b25c9-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="b25c9-117">Atualiza as propriedades de um objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b25c9-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b25c9-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b25c9-118">Properties</span></span>
|<span data-ttu-id="b25c9-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b25c9-119">Property</span></span>|<span data-ttu-id="b25c9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="b25c9-120">Type</span></span>|<span data-ttu-id="b25c9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b25c9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b25c9-122">id</span><span class="sxs-lookup"><span data-stu-id="b25c9-122">id</span></span>|<span data-ttu-id="b25c9-123">String</span><span class="sxs-lookup"><span data-stu-id="b25c9-123">String</span></span>|<span data-ttu-id="b25c9-124">ID da configuração do Office.</span><span class="sxs-lookup"><span data-stu-id="b25c9-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="b25c9-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="b25c9-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="b25c9-126">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b25c9-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="b25c9-127">Lista de status de check-in do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="b25c9-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="b25c9-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b25c9-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="b25c9-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b25c9-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="b25c9-130">Entidade que descreve o check-in do locatário Statues</span><span class="sxs-lookup"><span data-stu-id="b25c9-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="b25c9-131">Relações</span><span class="sxs-lookup"><span data-stu-id="b25c9-131">Relationships</span></span>
|<span data-ttu-id="b25c9-132">Relação</span><span class="sxs-lookup"><span data-stu-id="b25c9-132">Relationship</span></span>|<span data-ttu-id="b25c9-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b25c9-133">Type</span></span>|<span data-ttu-id="b25c9-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b25c9-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b25c9-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="b25c9-135">clientConfigurations</span></span>|<span data-ttu-id="b25c9-136">coleção [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b25c9-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="b25c9-137">Lista de configurações do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="b25c9-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b25c9-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b25c9-138">JSON Representation</span></span>
<span data-ttu-id="b25c9-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b25c9-139">Here is a JSON representation of the resource.</span></span>
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





