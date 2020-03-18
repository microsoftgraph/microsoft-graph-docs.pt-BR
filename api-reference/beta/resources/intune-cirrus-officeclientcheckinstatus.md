---
title: tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 66087cd47fa70352f8051fc220820ea355805f19
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797336"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="a9e18-103">tipo de recurso officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="a9e18-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="a9e18-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9e18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9e18-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9e18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9e18-106">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="a9e18-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="a9e18-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9e18-107">Properties</span></span>
|<span data-ttu-id="a9e18-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9e18-108">Property</span></span>|<span data-ttu-id="a9e18-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9e18-109">Type</span></span>|<span data-ttu-id="a9e18-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9e18-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9e18-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9e18-111">userPrincipalName</span></span>|<span data-ttu-id="a9e18-112">String</span><span class="sxs-lookup"><span data-stu-id="a9e18-112">String</span></span>|<span data-ttu-id="a9e18-113">Nome principal do usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9e18-113">User principal name using the device.</span></span>|
|<span data-ttu-id="a9e18-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="a9e18-114">deviceName</span></span>|<span data-ttu-id="a9e18-115">String</span><span class="sxs-lookup"><span data-stu-id="a9e18-115">String</span></span>|<span data-ttu-id="a9e18-116">Nome do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="a9e18-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="a9e18-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="a9e18-117">devicePlatform</span></span>|<span data-ttu-id="a9e18-118">String</span><span class="sxs-lookup"><span data-stu-id="a9e18-118">String</span></span>|<span data-ttu-id="a9e18-119">Plataforma do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="a9e18-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="a9e18-120">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="a9e18-120">devicePlatformVersion</span></span>|<span data-ttu-id="a9e18-121">String</span><span class="sxs-lookup"><span data-stu-id="a9e18-121">String</span></span>|<span data-ttu-id="a9e18-122">Versão da plataforma do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="a9e18-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="a9e18-123">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="a9e18-123">wasSuccessful</span></span>|<span data-ttu-id="a9e18-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9e18-124">Boolean</span></span>|<span data-ttu-id="a9e18-125">Se o último check-in foi bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="a9e18-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="a9e18-126">userId</span><span class="sxs-lookup"><span data-stu-id="a9e18-126">userId</span></span>|<span data-ttu-id="a9e18-127">String</span><span class="sxs-lookup"><span data-stu-id="a9e18-127">String</span></span>|<span data-ttu-id="a9e18-128">Identificador de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9e18-128">User identifier using the device.</span></span>|
|<span data-ttu-id="a9e18-129">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e18-129">checkinDateTime</span></span>|<span data-ttu-id="a9e18-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e18-130">DateTimeOffset</span></span>|<span data-ttu-id="a9e18-131">Tempo de check-in do último dispositivo em UTC.</span><span class="sxs-lookup"><span data-stu-id="a9e18-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="a9e18-132">errorMessage</span><span class="sxs-lookup"><span data-stu-id="a9e18-132">errorMessage</span></span>|<span data-ttu-id="a9e18-133">String</span><span class="sxs-lookup"><span data-stu-id="a9e18-133">String</span></span>|<span data-ttu-id="a9e18-134">Mensagem de erro se algum associado para o último check-in.</span><span class="sxs-lookup"><span data-stu-id="a9e18-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="a9e18-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="a9e18-135">appliedPolicies</span></span>|<span data-ttu-id="a9e18-136">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9e18-136">String collection</span></span>|<span data-ttu-id="a9e18-137">Lista de políticas entregues ao dispositivo como última verificação.</span><span class="sxs-lookup"><span data-stu-id="a9e18-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9e18-138">Relações</span><span class="sxs-lookup"><span data-stu-id="a9e18-138">Relationships</span></span>
<span data-ttu-id="a9e18-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a9e18-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9e18-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9e18-140">JSON Representation</span></span>
<span data-ttu-id="a9e18-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9e18-141">Here is a JSON representation of the resource.</span></span>
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



