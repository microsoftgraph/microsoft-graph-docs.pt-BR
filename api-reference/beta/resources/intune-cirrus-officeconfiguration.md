---
title: tipo de recurso officeConfiguration
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e5c36a23be0ab32a14a08eaff297b832ba5274c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526353"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="8d476-103">tipo de recurso officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d476-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="8d476-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d476-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d476-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d476-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d476-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8d476-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="8d476-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8d476-107">Methods</span></span>
|<span data-ttu-id="8d476-108">Método</span><span class="sxs-lookup"><span data-stu-id="8d476-108">Method</span></span>|<span data-ttu-id="8d476-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d476-109">Return Type</span></span>|<span data-ttu-id="8d476-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d476-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d476-111">Obter officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d476-111">Get officeConfiguration</span></span>|[<span data-ttu-id="8d476-112">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d476-112">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="8d476-113">Leia as propriedades e as relações do objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8d476-113">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="8d476-114">Atualizar officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d476-114">Update officeConfiguration</span></span>|[<span data-ttu-id="8d476-115">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d476-115">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="8d476-116">Atualiza as propriedades de um objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8d476-116">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d476-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d476-117">Properties</span></span>
|<span data-ttu-id="8d476-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d476-118">Property</span></span>|<span data-ttu-id="8d476-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d476-119">Type</span></span>|<span data-ttu-id="8d476-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d476-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d476-121">id</span><span class="sxs-lookup"><span data-stu-id="8d476-121">id</span></span>|<span data-ttu-id="8d476-122">String</span><span class="sxs-lookup"><span data-stu-id="8d476-122">String</span></span>|<span data-ttu-id="8d476-123">ID da configuração do Office.</span><span class="sxs-lookup"><span data-stu-id="8d476-123">Id of the office configuration.</span></span>|
|<span data-ttu-id="8d476-124">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="8d476-124">tenantCheckinStatuses</span></span>|<span data-ttu-id="8d476-125">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8d476-125">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="8d476-126">Lista de status de check-in do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="8d476-126">List of office Client check-in status.</span></span>|
|<span data-ttu-id="8d476-127">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="8d476-127">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="8d476-128">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="8d476-128">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="8d476-129">Entidade que descreve o check-in do locatário Statues</span><span class="sxs-lookup"><span data-stu-id="8d476-129">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d476-130">Relações</span><span class="sxs-lookup"><span data-stu-id="8d476-130">Relationships</span></span>
|<span data-ttu-id="8d476-131">Relação</span><span class="sxs-lookup"><span data-stu-id="8d476-131">Relationship</span></span>|<span data-ttu-id="8d476-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d476-132">Type</span></span>|<span data-ttu-id="8d476-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d476-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d476-134">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="8d476-134">clientConfigurations</span></span>|<span data-ttu-id="8d476-135">coleção [conjuntoofficeclientconfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d476-135">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="8d476-136">Lista de configurações do cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="8d476-136">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d476-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d476-137">JSON Representation</span></span>
<span data-ttu-id="8d476-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d476-138">Here is a JSON representation of the resource.</span></span>
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



