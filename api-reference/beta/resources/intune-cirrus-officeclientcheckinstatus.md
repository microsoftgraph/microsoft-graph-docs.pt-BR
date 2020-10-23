---
title: tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 014246b973e9ea94ef79eba45c771110dca6da76
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694008"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="f8c87-103">tipo de recurso officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="f8c87-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="f8c87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8c87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8c87-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f8c87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8c87-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8c87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8c87-107">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="f8c87-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="f8c87-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8c87-108">Properties</span></span>
|<span data-ttu-id="f8c87-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8c87-109">Property</span></span>|<span data-ttu-id="f8c87-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8c87-110">Type</span></span>|<span data-ttu-id="f8c87-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8c87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8c87-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8c87-112">userPrincipalName</span></span>|<span data-ttu-id="f8c87-113">String</span><span class="sxs-lookup"><span data-stu-id="f8c87-113">String</span></span>|<span data-ttu-id="f8c87-114">Nome principal do usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8c87-114">User principal name using the device.</span></span>|
|<span data-ttu-id="f8c87-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="f8c87-115">deviceName</span></span>|<span data-ttu-id="f8c87-116">String</span><span class="sxs-lookup"><span data-stu-id="f8c87-116">String</span></span>|<span data-ttu-id="f8c87-117">Nome do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="f8c87-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="f8c87-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="f8c87-118">devicePlatform</span></span>|<span data-ttu-id="f8c87-119">String</span><span class="sxs-lookup"><span data-stu-id="f8c87-119">String</span></span>|<span data-ttu-id="f8c87-120">Plataforma do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="f8c87-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="f8c87-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="f8c87-121">devicePlatformVersion</span></span>|<span data-ttu-id="f8c87-122">String</span><span class="sxs-lookup"><span data-stu-id="f8c87-122">String</span></span>|<span data-ttu-id="f8c87-123">Versão da plataforma do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="f8c87-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="f8c87-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="f8c87-124">wasSuccessful</span></span>|<span data-ttu-id="f8c87-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8c87-125">Boolean</span></span>|<span data-ttu-id="f8c87-126">Se o último check-in foi bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="f8c87-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="f8c87-127">userId</span><span class="sxs-lookup"><span data-stu-id="f8c87-127">userId</span></span>|<span data-ttu-id="f8c87-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8c87-128">String</span></span>|<span data-ttu-id="f8c87-129">Identificador de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8c87-129">User identifier using the device.</span></span>|
|<span data-ttu-id="f8c87-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="f8c87-130">checkinDateTime</span></span>|<span data-ttu-id="f8c87-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8c87-131">DateTimeOffset</span></span>|<span data-ttu-id="f8c87-132">Tempo de check-in do último dispositivo em UTC.</span><span class="sxs-lookup"><span data-stu-id="f8c87-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="f8c87-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="f8c87-133">errorMessage</span></span>|<span data-ttu-id="f8c87-134">String</span><span class="sxs-lookup"><span data-stu-id="f8c87-134">String</span></span>|<span data-ttu-id="f8c87-135">Mensagem de erro se algum associado para o último check-in.</span><span class="sxs-lookup"><span data-stu-id="f8c87-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="f8c87-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="f8c87-136">appliedPolicies</span></span>|<span data-ttu-id="f8c87-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f8c87-137">String collection</span></span>|<span data-ttu-id="f8c87-138">Lista de políticas entregues ao dispositivo como última verificação.</span><span class="sxs-lookup"><span data-stu-id="f8c87-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8c87-139">Relações</span><span class="sxs-lookup"><span data-stu-id="f8c87-139">Relationships</span></span>
<span data-ttu-id="f8c87-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8c87-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8c87-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8c87-141">JSON Representation</span></span>
<span data-ttu-id="f8c87-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8c87-142">Here is a JSON representation of the resource.</span></span>
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





