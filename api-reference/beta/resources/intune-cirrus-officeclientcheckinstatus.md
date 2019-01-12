---
title: tipo de recurso de officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do inquilino.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a387e04b9ebc15d65eb8dd883ecd4a9bae78ad6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969286"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="35071-103">tipo de recurso de officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="35071-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="35071-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="35071-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35071-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="35071-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35071-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="35071-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35071-107">Entidade que descreve as estatísticas de check-in do inquilino.</span><span class="sxs-lookup"><span data-stu-id="35071-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="35071-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35071-108">Properties</span></span>
|<span data-ttu-id="35071-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35071-109">Property</span></span>|<span data-ttu-id="35071-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="35071-110">Type</span></span>|<span data-ttu-id="35071-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="35071-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35071-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="35071-112">userPrincipalName</span></span>|<span data-ttu-id="35071-113">String</span><span class="sxs-lookup"><span data-stu-id="35071-113">String</span></span>|<span data-ttu-id="35071-114">Nome principal de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35071-114">User principal name using the device.</span></span>|
|<span data-ttu-id="35071-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="35071-115">deviceName</span></span>|<span data-ttu-id="35071-116">String</span><span class="sxs-lookup"><span data-stu-id="35071-116">String</span></span>|<span data-ttu-id="35071-117">Nome do dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="35071-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="35071-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="35071-118">devicePlatform</span></span>|<span data-ttu-id="35071-119">String</span><span class="sxs-lookup"><span data-stu-id="35071-119">String</span></span>|<span data-ttu-id="35071-120">Plataforma de dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="35071-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="35071-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="35071-121">devicePlatformVersion</span></span>|<span data-ttu-id="35071-122">String</span><span class="sxs-lookup"><span data-stu-id="35071-122">String</span></span>|<span data-ttu-id="35071-123">Versão de plataforma do dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="35071-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="35071-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="35071-124">wasSuccessful</span></span>|<span data-ttu-id="35071-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="35071-125">Boolean</span></span>|<span data-ttu-id="35071-126">Se o último check-in foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="35071-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="35071-127">userId</span><span class="sxs-lookup"><span data-stu-id="35071-127">userId</span></span>|<span data-ttu-id="35071-128">String</span><span class="sxs-lookup"><span data-stu-id="35071-128">String</span></span>|<span data-ttu-id="35071-129">Identificador de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35071-129">User identifier using the device.</span></span>|
|<span data-ttu-id="35071-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="35071-130">checkinDateTime</span></span>|<span data-ttu-id="35071-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35071-131">DateTimeOffset</span></span>|<span data-ttu-id="35071-132">Último dispositivo tempo check-in em UTC.</span><span class="sxs-lookup"><span data-stu-id="35071-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="35071-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="35071-133">errorMessage</span></span>|<span data-ttu-id="35071-134">String</span><span class="sxs-lookup"><span data-stu-id="35071-134">String</span></span>|<span data-ttu-id="35071-135">Mensagem de erro, se houver algum associado para o último check-in.</span><span class="sxs-lookup"><span data-stu-id="35071-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="35071-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="35071-136">appliedPolicies</span></span>|<span data-ttu-id="35071-137">String collection</span><span class="sxs-lookup"><span data-stu-id="35071-137">String collection</span></span>|<span data-ttu-id="35071-138">Lista de políticas entregues ao dispositivo como último check-in.</span><span class="sxs-lookup"><span data-stu-id="35071-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35071-139">Relações</span><span class="sxs-lookup"><span data-stu-id="35071-139">Relationships</span></span>
<span data-ttu-id="35071-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35071-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="35071-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35071-141">JSON Representation</span></span>
<span data-ttu-id="35071-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35071-142">Here is a JSON representation of the resource.</span></span>
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



