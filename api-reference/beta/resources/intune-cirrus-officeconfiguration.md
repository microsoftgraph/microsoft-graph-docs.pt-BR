---
title: tipo de recurso de officeConfiguration
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: tfitzmac
ms.openlocfilehash: bf74789d4debda00b21173ff2974db8224cd15f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305541"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="9c206-103">tipo de recurso de officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c206-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="9c206-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9c206-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c206-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9c206-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c206-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9c206-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c206-107">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9c206-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="9c206-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9c206-108">Methods</span></span>
|<span data-ttu-id="9c206-109">Método</span><span class="sxs-lookup"><span data-stu-id="9c206-109">Method</span></span>|<span data-ttu-id="9c206-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9c206-110">Return Type</span></span>|<span data-ttu-id="9c206-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c206-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c206-112">Obter officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c206-112">Get officeConfiguration</span></span>|[<span data-ttu-id="9c206-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c206-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="9c206-114">Leia as propriedades e os relacionamentos do objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9c206-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="9c206-115">Atualizar officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c206-115">Update officeConfiguration</span></span>|[<span data-ttu-id="9c206-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c206-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="9c206-117">Atualize as propriedades de um objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9c206-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c206-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c206-118">Properties</span></span>
|<span data-ttu-id="9c206-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c206-119">Property</span></span>|<span data-ttu-id="9c206-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c206-120">Type</span></span>|<span data-ttu-id="9c206-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c206-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c206-122">id</span><span class="sxs-lookup"><span data-stu-id="9c206-122">id</span></span>|<span data-ttu-id="9c206-123">String</span><span class="sxs-lookup"><span data-stu-id="9c206-123">String</span></span>|<span data-ttu-id="9c206-124">ID da configuração do office.</span><span class="sxs-lookup"><span data-stu-id="9c206-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="9c206-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="9c206-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="9c206-126">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="9c206-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="9c206-127">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="9c206-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="9c206-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="9c206-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="9c206-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="9c206-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="9c206-130">Entidade que descreve o locatário check-in statues</span><span class="sxs-lookup"><span data-stu-id="9c206-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c206-131">Relações</span><span class="sxs-lookup"><span data-stu-id="9c206-131">Relationships</span></span>
|<span data-ttu-id="9c206-132">Relação</span><span class="sxs-lookup"><span data-stu-id="9c206-132">Relationship</span></span>|<span data-ttu-id="9c206-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c206-133">Type</span></span>|<span data-ttu-id="9c206-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c206-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c206-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="9c206-135">clientConfigurations</span></span>|<span data-ttu-id="9c206-136">coleção [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9c206-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="9c206-137">Lista de configuração de cliente do office.</span><span class="sxs-lookup"><span data-stu-id="9c206-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c206-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c206-138">JSON Representation</span></span>
<span data-ttu-id="9c206-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c206-139">Here is a JSON representation of the resource.</span></span>
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



