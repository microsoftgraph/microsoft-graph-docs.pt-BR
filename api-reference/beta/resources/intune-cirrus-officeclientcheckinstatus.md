---
title: tipo de recurso de officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do inquilino.
ms.openlocfilehash: a87a085d42ce0754e046b319b270ddf90a3bdba7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035755"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="c2fd4-103">tipo de recurso de officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="c2fd4-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="c2fd4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2fd4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2fd4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2fd4-107">Entidade que descreve as estatísticas de check-in do inquilino.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="c2fd4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2fd4-108">Properties</span></span>
|<span data-ttu-id="c2fd4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2fd4-109">Property</span></span>|<span data-ttu-id="c2fd4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2fd4-110">Type</span></span>|<span data-ttu-id="c2fd4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2fd4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2fd4-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c2fd4-112">userPrincipalName</span></span>|<span data-ttu-id="c2fd4-113">String</span><span class="sxs-lookup"><span data-stu-id="c2fd4-113">String</span></span>|<span data-ttu-id="c2fd4-114">Nome principal de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-114">User principal name using the device.</span></span>|
|<span data-ttu-id="c2fd4-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="c2fd4-115">deviceName</span></span>|<span data-ttu-id="c2fd4-116">String</span><span class="sxs-lookup"><span data-stu-id="c2fd4-116">String</span></span>|<span data-ttu-id="c2fd4-117">Nome do dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="c2fd4-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="c2fd4-118">devicePlatform</span></span>|<span data-ttu-id="c2fd4-119">String</span><span class="sxs-lookup"><span data-stu-id="c2fd4-119">String</span></span>|<span data-ttu-id="c2fd4-120">Plataforma de dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="c2fd4-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="c2fd4-121">devicePlatformVersion</span></span>|<span data-ttu-id="c2fd4-122">String</span><span class="sxs-lookup"><span data-stu-id="c2fd4-122">String</span></span>|<span data-ttu-id="c2fd4-123">Versão de plataforma do dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="c2fd4-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="c2fd4-124">wasSuccessful</span></span>|<span data-ttu-id="c2fd4-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="c2fd4-125">Boolean</span></span>|<span data-ttu-id="c2fd4-126">Se o último check-in foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="c2fd4-127">userId</span><span class="sxs-lookup"><span data-stu-id="c2fd4-127">userId</span></span>|<span data-ttu-id="c2fd4-128">String</span><span class="sxs-lookup"><span data-stu-id="c2fd4-128">String</span></span>|<span data-ttu-id="c2fd4-129">Identificador de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-129">User identifier using the device.</span></span>|
|<span data-ttu-id="c2fd4-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="c2fd4-130">checkinDateTime</span></span>|<span data-ttu-id="c2fd4-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2fd4-131">DateTimeOffset</span></span>|<span data-ttu-id="c2fd4-132">Último dispositivo tempo check-in em UTC.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="c2fd4-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="c2fd4-133">errorMessage</span></span>|<span data-ttu-id="c2fd4-134">String</span><span class="sxs-lookup"><span data-stu-id="c2fd4-134">String</span></span>|<span data-ttu-id="c2fd4-135">Mensagem de erro, se houver algum associado para o último check-in.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="c2fd4-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c2fd4-136">appliedPolicies</span></span>|<span data-ttu-id="c2fd4-137">String collection</span><span class="sxs-lookup"><span data-stu-id="c2fd4-137">String collection</span></span>|<span data-ttu-id="c2fd4-138">Lista de políticas entregues ao dispositivo como último check-in.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2fd4-139">Relações</span><span class="sxs-lookup"><span data-stu-id="c2fd4-139">Relationships</span></span>
<span data-ttu-id="c2fd4-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2fd4-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2fd4-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2fd4-141">JSON Representation</span></span>
<span data-ttu-id="c2fd4-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2fd4-142">Here is a JSON representation of the resource.</span></span>
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



