---
title: tipo de recurso de officeConfiguration
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc76295b21602328689ee48f8aed8be74bd82093
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406546"
---
# <a name="officeconfiguration-resource-type"></a><span data-ttu-id="cc41a-103">tipo de recurso de officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc41a-103">officeConfiguration resource type</span></span>

> <span data-ttu-id="cc41a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="cc41a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc41a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cc41a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc41a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="cc41a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc41a-107">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cc41a-107">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="cc41a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cc41a-108">Methods</span></span>
|<span data-ttu-id="cc41a-109">Método</span><span class="sxs-lookup"><span data-stu-id="cc41a-109">Method</span></span>|<span data-ttu-id="cc41a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc41a-110">Return Type</span></span>|<span data-ttu-id="cc41a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc41a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc41a-112">Obter officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc41a-112">Get officeConfiguration</span></span>|[<span data-ttu-id="cc41a-113">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc41a-113">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="cc41a-114">Leia as propriedades e os relacionamentos do objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cc41a-114">Read properties and relationships of the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|
|<span data-ttu-id="cc41a-115">Atualizar officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc41a-115">Update officeConfiguration</span></span>|[<span data-ttu-id="cc41a-116">officeConfiguration</span><span class="sxs-lookup"><span data-stu-id="cc41a-116">officeConfiguration</span></span>](../resources/intune-cirrus-officeconfiguration.md)|<span data-ttu-id="cc41a-117">Atualize as propriedades de um objeto [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="cc41a-117">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc41a-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc41a-118">Properties</span></span>
|<span data-ttu-id="cc41a-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc41a-119">Property</span></span>|<span data-ttu-id="cc41a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc41a-120">Type</span></span>|<span data-ttu-id="cc41a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc41a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc41a-122">id</span><span class="sxs-lookup"><span data-stu-id="cc41a-122">id</span></span>|<span data-ttu-id="cc41a-123">String</span><span class="sxs-lookup"><span data-stu-id="cc41a-123">String</span></span>|<span data-ttu-id="cc41a-124">ID da configuração do office.</span><span class="sxs-lookup"><span data-stu-id="cc41a-124">Id of the office configuration.</span></span>|
|<span data-ttu-id="cc41a-125">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="cc41a-125">tenantCheckinStatuses</span></span>|<span data-ttu-id="cc41a-126">coleção [officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)</span><span class="sxs-lookup"><span data-stu-id="cc41a-126">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="cc41a-127">Lista de status de check-in do cliente do office.</span><span class="sxs-lookup"><span data-stu-id="cc41a-127">List of office Client check-in status.</span></span>|
|<span data-ttu-id="cc41a-128">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="cc41a-128">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="cc41a-129">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="cc41a-129">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="cc41a-130">Entidade que descreve o locatário check-in statues</span><span class="sxs-lookup"><span data-stu-id="cc41a-130">Entity that describes tenant check-in statues</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc41a-131">Relações</span><span class="sxs-lookup"><span data-stu-id="cc41a-131">Relationships</span></span>
|<span data-ttu-id="cc41a-132">Relação</span><span class="sxs-lookup"><span data-stu-id="cc41a-132">Relationship</span></span>|<span data-ttu-id="cc41a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc41a-133">Type</span></span>|<span data-ttu-id="cc41a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc41a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc41a-135">clientConfigurations</span><span class="sxs-lookup"><span data-stu-id="cc41a-135">clientConfigurations</span></span>|<span data-ttu-id="cc41a-136">coleção [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cc41a-136">[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) collection</span></span>|<span data-ttu-id="cc41a-137">Lista de configuração de cliente do office.</span><span class="sxs-lookup"><span data-stu-id="cc41a-137">List of office Client configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc41a-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc41a-138">JSON Representation</span></span>
<span data-ttu-id="cc41a-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc41a-139">Here is a JSON representation of the resource.</span></span>
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



