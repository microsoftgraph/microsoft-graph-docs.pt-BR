---
title: tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 647d55e3d5eca6acb47b90092dc0502097b63cf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021760"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="c7e13-103">tipo de recurso officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="c7e13-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="c7e13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7e13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7e13-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c7e13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7e13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c7e13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e13-107">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="c7e13-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="c7e13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7e13-108">Properties</span></span>
|<span data-ttu-id="c7e13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7e13-109">Property</span></span>|<span data-ttu-id="c7e13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7e13-110">Type</span></span>|<span data-ttu-id="c7e13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7e13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e13-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7e13-112">userPrincipalName</span></span>|<span data-ttu-id="c7e13-113">String</span><span class="sxs-lookup"><span data-stu-id="c7e13-113">String</span></span>|<span data-ttu-id="c7e13-114">Nome principal do usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7e13-114">User principal name using the device.</span></span>|
|<span data-ttu-id="c7e13-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="c7e13-115">deviceName</span></span>|<span data-ttu-id="c7e13-116">String</span><span class="sxs-lookup"><span data-stu-id="c7e13-116">String</span></span>|<span data-ttu-id="c7e13-117">Nome do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c7e13-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="c7e13-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="c7e13-118">devicePlatform</span></span>|<span data-ttu-id="c7e13-119">String</span><span class="sxs-lookup"><span data-stu-id="c7e13-119">String</span></span>|<span data-ttu-id="c7e13-120">Plataforma do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c7e13-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="c7e13-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="c7e13-121">devicePlatformVersion</span></span>|<span data-ttu-id="c7e13-122">String</span><span class="sxs-lookup"><span data-stu-id="c7e13-122">String</span></span>|<span data-ttu-id="c7e13-123">Versão da plataforma do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c7e13-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="c7e13-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="c7e13-124">wasSuccessful</span></span>|<span data-ttu-id="c7e13-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="c7e13-125">Boolean</span></span>|<span data-ttu-id="c7e13-126">Se o último check-in foi bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="c7e13-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="c7e13-127">userId</span><span class="sxs-lookup"><span data-stu-id="c7e13-127">userId</span></span>|<span data-ttu-id="c7e13-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7e13-128">String</span></span>|<span data-ttu-id="c7e13-129">Identificador de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c7e13-129">User identifier using the device.</span></span>|
|<span data-ttu-id="c7e13-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="c7e13-130">checkinDateTime</span></span>|<span data-ttu-id="c7e13-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7e13-131">DateTimeOffset</span></span>|<span data-ttu-id="c7e13-132">Tempo de check-in do último dispositivo em UTC.</span><span class="sxs-lookup"><span data-stu-id="c7e13-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="c7e13-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="c7e13-133">errorMessage</span></span>|<span data-ttu-id="c7e13-134">String</span><span class="sxs-lookup"><span data-stu-id="c7e13-134">String</span></span>|<span data-ttu-id="c7e13-135">Mensagem de erro se algum associado para o último check-in.</span><span class="sxs-lookup"><span data-stu-id="c7e13-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="c7e13-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c7e13-136">appliedPolicies</span></span>|<span data-ttu-id="c7e13-137">Coleção String</span><span class="sxs-lookup"><span data-stu-id="c7e13-137">String collection</span></span>|<span data-ttu-id="c7e13-138">Lista de políticas entregues ao dispositivo como última verificação.</span><span class="sxs-lookup"><span data-stu-id="c7e13-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7e13-139">Relações</span><span class="sxs-lookup"><span data-stu-id="c7e13-139">Relationships</span></span>
<span data-ttu-id="c7e13-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7e13-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7e13-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7e13-141">JSON Representation</span></span>
<span data-ttu-id="c7e13-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7e13-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
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
```






