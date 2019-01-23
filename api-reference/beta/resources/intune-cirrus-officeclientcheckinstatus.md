---
title: tipo de recurso de officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do inquilino.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403256"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="f97f6-103">tipo de recurso de officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="f97f6-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="f97f6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f97f6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f97f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f97f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f97f6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f97f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f97f6-107">Entidade que descreve as estatísticas de check-in do inquilino.</span><span class="sxs-lookup"><span data-stu-id="f97f6-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="f97f6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f97f6-108">Properties</span></span>
|<span data-ttu-id="f97f6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f97f6-109">Property</span></span>|<span data-ttu-id="f97f6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f97f6-110">Type</span></span>|<span data-ttu-id="f97f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f97f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f97f6-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f97f6-112">userPrincipalName</span></span>|<span data-ttu-id="f97f6-113">String</span><span class="sxs-lookup"><span data-stu-id="f97f6-113">String</span></span>|<span data-ttu-id="f97f6-114">Nome principal de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f97f6-114">User principal name using the device.</span></span>|
|<span data-ttu-id="f97f6-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="f97f6-115">deviceName</span></span>|<span data-ttu-id="f97f6-116">String</span><span class="sxs-lookup"><span data-stu-id="f97f6-116">String</span></span>|<span data-ttu-id="f97f6-117">Nome do dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="f97f6-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="f97f6-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="f97f6-118">devicePlatform</span></span>|<span data-ttu-id="f97f6-119">String</span><span class="sxs-lookup"><span data-stu-id="f97f6-119">String</span></span>|<span data-ttu-id="f97f6-120">Plataforma de dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="f97f6-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="f97f6-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="f97f6-121">devicePlatformVersion</span></span>|<span data-ttu-id="f97f6-122">String</span><span class="sxs-lookup"><span data-stu-id="f97f6-122">String</span></span>|<span data-ttu-id="f97f6-123">Versão de plataforma do dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="f97f6-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="f97f6-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="f97f6-124">wasSuccessful</span></span>|<span data-ttu-id="f97f6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="f97f6-125">Boolean</span></span>|<span data-ttu-id="f97f6-126">Se o último check-in foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f97f6-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="f97f6-127">userId</span><span class="sxs-lookup"><span data-stu-id="f97f6-127">userId</span></span>|<span data-ttu-id="f97f6-128">String</span><span class="sxs-lookup"><span data-stu-id="f97f6-128">String</span></span>|<span data-ttu-id="f97f6-129">Identificador de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f97f6-129">User identifier using the device.</span></span>|
|<span data-ttu-id="f97f6-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="f97f6-130">checkinDateTime</span></span>|<span data-ttu-id="f97f6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f97f6-131">DateTimeOffset</span></span>|<span data-ttu-id="f97f6-132">Último dispositivo tempo check-in em UTC.</span><span class="sxs-lookup"><span data-stu-id="f97f6-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="f97f6-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="f97f6-133">errorMessage</span></span>|<span data-ttu-id="f97f6-134">String</span><span class="sxs-lookup"><span data-stu-id="f97f6-134">String</span></span>|<span data-ttu-id="f97f6-135">Mensagem de erro, se houver algum associado para o último check-in.</span><span class="sxs-lookup"><span data-stu-id="f97f6-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="f97f6-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="f97f6-136">appliedPolicies</span></span>|<span data-ttu-id="f97f6-137">String collection</span><span class="sxs-lookup"><span data-stu-id="f97f6-137">String collection</span></span>|<span data-ttu-id="f97f6-138">Lista de políticas entregues ao dispositivo como último check-in.</span><span class="sxs-lookup"><span data-stu-id="f97f6-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f97f6-139">Relações</span><span class="sxs-lookup"><span data-stu-id="f97f6-139">Relationships</span></span>
<span data-ttu-id="f97f6-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f97f6-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f97f6-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f97f6-141">JSON Representation</span></span>
<span data-ttu-id="f97f6-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f97f6-142">Here is a JSON representation of the resource.</span></span>
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



