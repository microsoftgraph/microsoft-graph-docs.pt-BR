---
title: tipo de recurso de officeConfiguration
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 767782e26dd203e2ab5488b30520d8cbcf44d1e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921357"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="d18bc-103">tipo de recurso de officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d18bc-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="d18bc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d18bc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d18bc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d18bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d18bc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d18bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d18bc-107">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d18bc-107">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="d18bc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="d18bc-108">Methods</span></span>
|<span data-ttu-id="d18bc-109">Método</span><span class="sxs-lookup"><span data-stu-id="d18bc-109">Method</span></span>|<span data-ttu-id="d18bc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d18bc-110">Return Type</span></span>|<span data-ttu-id="d18bc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d18bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d18bc-112">Obter officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d18bc-112">Get officeConfiguration</span></span>|[<span data-ttu-id="d18bc-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d18bc-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="d18bc-114">Leia as propriedades e os relacionamentos do objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d18bc-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="d18bc-115">Atualizar officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d18bc-115">Update officeConfiguration</span></span>|[<span data-ttu-id="d18bc-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d18bc-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="d18bc-117">Atualize as propriedades de um objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d18bc-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d18bc-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d18bc-118">Properties</span></span>
|<span data-ttu-id="d18bc-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d18bc-119">Property</span></span>|<span data-ttu-id="d18bc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d18bc-120">Type</span></span>|<span data-ttu-id="d18bc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d18bc-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d18bc-122">id</span><span class="sxs-lookup"><span data-stu-id="d18bc-122">id</span></span>|<span data-ttu-id="d18bc-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d18bc-123">String</span></span>|<span data-ttu-id="d18bc-124">ID da configuração do office.</span><span class="sxs-lookup"><span data-stu-id="d18bc-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="d18bc-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="d18bc-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="d18bc-126">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="d18bc-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="d18bc-127">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="d18bc-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="d18bc-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d18bc-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="d18bc-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="d18bc-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="d18bc-130">Entidade que descreve o locatário check-in statues</span><span class="sxs-lookup"><span data-stu-id="d18bc-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="d18bc-131">Relações</span><span class="sxs-lookup"><span data-stu-id="d18bc-131">Relationships</span></span>
|<span data-ttu-id="d18bc-132">Relação</span><span class="sxs-lookup"><span data-stu-id="d18bc-132">Relationship</span></span>|<span data-ttu-id="d18bc-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d18bc-133">Type</span></span>|<span data-ttu-id="d18bc-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d18bc-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d18bc-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="d18bc-135">clientConfigurations</span></span>|<span data-ttu-id="d18bc-136">coleção [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d18bc-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="d18bc-137">Lista de configuração de cliente do office.</span><span class="sxs-lookup"><span data-stu-id="d18bc-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d18bc-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d18bc-138">JSON Representation</span></span>
<span data-ttu-id="d18bc-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d18bc-139">Here is a JSON representation of the resource.</span></span>
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



