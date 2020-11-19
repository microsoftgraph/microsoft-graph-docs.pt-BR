---
title: tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdd2d4f47244bb2eab1e7c357a9f599909166b6a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295121"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="c672f-103">tipo de recurso officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="c672f-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="c672f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c672f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c672f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c672f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c672f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c672f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c672f-107">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="c672f-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="c672f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c672f-108">Properties</span></span>
|<span data-ttu-id="c672f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c672f-109">Property</span></span>|<span data-ttu-id="c672f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c672f-110">Type</span></span>|<span data-ttu-id="c672f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c672f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c672f-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c672f-112">userPrincipalName</span></span>|<span data-ttu-id="c672f-113">String</span><span class="sxs-lookup"><span data-stu-id="c672f-113">String</span></span>|<span data-ttu-id="c672f-114">Nome principal do usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c672f-114">User principal name using the device.</span></span>|
|<span data-ttu-id="c672f-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="c672f-115">deviceName</span></span>|<span data-ttu-id="c672f-116">String</span><span class="sxs-lookup"><span data-stu-id="c672f-116">String</span></span>|<span data-ttu-id="c672f-117">Nome do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c672f-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="c672f-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="c672f-118">devicePlatform</span></span>|<span data-ttu-id="c672f-119">String</span><span class="sxs-lookup"><span data-stu-id="c672f-119">String</span></span>|<span data-ttu-id="c672f-120">Plataforma do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c672f-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="c672f-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="c672f-121">devicePlatformVersion</span></span>|<span data-ttu-id="c672f-122">String</span><span class="sxs-lookup"><span data-stu-id="c672f-122">String</span></span>|<span data-ttu-id="c672f-123">Versão da plataforma do dispositivo que está tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c672f-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="c672f-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="c672f-124">wasSuccessful</span></span>|<span data-ttu-id="c672f-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="c672f-125">Boolean</span></span>|<span data-ttu-id="c672f-126">Se o último check-in foi bem-sucedido.</span><span class="sxs-lookup"><span data-stu-id="c672f-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="c672f-127">userId</span><span class="sxs-lookup"><span data-stu-id="c672f-127">userId</span></span>|<span data-ttu-id="c672f-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c672f-128">String</span></span>|<span data-ttu-id="c672f-129">Identificador de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c672f-129">User identifier using the device.</span></span>|
|<span data-ttu-id="c672f-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="c672f-130">checkinDateTime</span></span>|<span data-ttu-id="c672f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c672f-131">DateTimeOffset</span></span>|<span data-ttu-id="c672f-132">Tempo de check-in do último dispositivo em UTC.</span><span class="sxs-lookup"><span data-stu-id="c672f-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="c672f-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="c672f-133">errorMessage</span></span>|<span data-ttu-id="c672f-134">String</span><span class="sxs-lookup"><span data-stu-id="c672f-134">String</span></span>|<span data-ttu-id="c672f-135">Mensagem de erro se algum associado para o último check-in.</span><span class="sxs-lookup"><span data-stu-id="c672f-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="c672f-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c672f-136">appliedPolicies</span></span>|<span data-ttu-id="c672f-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c672f-137">String collection</span></span>|<span data-ttu-id="c672f-138">Lista de políticas entregues ao dispositivo como última verificação.</span><span class="sxs-lookup"><span data-stu-id="c672f-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c672f-139">Relações</span><span class="sxs-lookup"><span data-stu-id="c672f-139">Relationships</span></span>
<span data-ttu-id="c672f-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c672f-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c672f-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c672f-141">JSON Representation</span></span>
<span data-ttu-id="c672f-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c672f-142">Here is a JSON representation of the resource.</span></span>
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




