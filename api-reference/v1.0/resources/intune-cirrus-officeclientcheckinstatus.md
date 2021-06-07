---
title: Tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdd2d4f47244bb2eab1e7c357a9f599909166b6a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758492"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="359c6-103">Tipo de recurso officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="359c6-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="359c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="359c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="359c6-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="359c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="359c6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="359c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="359c6-107">Entidade que descreve as estatísticas de check-in do locatário.</span><span class="sxs-lookup"><span data-stu-id="359c6-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="359c6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="359c6-108">Properties</span></span>
|<span data-ttu-id="359c6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="359c6-109">Property</span></span>|<span data-ttu-id="359c6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="359c6-110">Type</span></span>|<span data-ttu-id="359c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="359c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="359c6-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="359c6-112">userPrincipalName</span></span>|<span data-ttu-id="359c6-113">String</span><span class="sxs-lookup"><span data-stu-id="359c6-113">String</span></span>|<span data-ttu-id="359c6-114">Nome principal do usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="359c6-114">User principal name using the device.</span></span>|
|<span data-ttu-id="359c6-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="359c6-115">deviceName</span></span>|<span data-ttu-id="359c6-116">String</span><span class="sxs-lookup"><span data-stu-id="359c6-116">String</span></span>|<span data-ttu-id="359c6-117">Nome do dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="359c6-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="359c6-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="359c6-118">devicePlatform</span></span>|<span data-ttu-id="359c6-119">String</span><span class="sxs-lookup"><span data-stu-id="359c6-119">String</span></span>|<span data-ttu-id="359c6-120">Plataforma de dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="359c6-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="359c6-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="359c6-121">devicePlatformVersion</span></span>|<span data-ttu-id="359c6-122">String</span><span class="sxs-lookup"><span data-stu-id="359c6-122">String</span></span>|<span data-ttu-id="359c6-123">Versão da plataforma do dispositivo tentando fazer check-in.</span><span class="sxs-lookup"><span data-stu-id="359c6-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="359c6-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="359c6-124">wasSuccessful</span></span>|<span data-ttu-id="359c6-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="359c6-125">Boolean</span></span>|<span data-ttu-id="359c6-126">Se a última verificação tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="359c6-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="359c6-127">userId</span><span class="sxs-lookup"><span data-stu-id="359c6-127">userId</span></span>|<span data-ttu-id="359c6-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="359c6-128">String</span></span>|<span data-ttu-id="359c6-129">Identificador de usuário usando o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="359c6-129">User identifier using the device.</span></span>|
|<span data-ttu-id="359c6-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="359c6-130">checkinDateTime</span></span>|<span data-ttu-id="359c6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="359c6-131">DateTimeOffset</span></span>|<span data-ttu-id="359c6-132">Última hora de check-in do dispositivo em UTC.</span><span class="sxs-lookup"><span data-stu-id="359c6-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="359c6-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="359c6-133">errorMessage</span></span>|<span data-ttu-id="359c6-134">String</span><span class="sxs-lookup"><span data-stu-id="359c6-134">String</span></span>|<span data-ttu-id="359c6-135">Mensagem de erro se alguma associada ao último check-in.</span><span class="sxs-lookup"><span data-stu-id="359c6-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="359c6-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="359c6-136">appliedPolicies</span></span>|<span data-ttu-id="359c6-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="359c6-137">String collection</span></span>|<span data-ttu-id="359c6-138">Lista de políticas entregues ao dispositivo como última verificação.</span><span class="sxs-lookup"><span data-stu-id="359c6-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="359c6-139">Relações</span><span class="sxs-lookup"><span data-stu-id="359c6-139">Relationships</span></span>
<span data-ttu-id="359c6-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="359c6-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="359c6-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="359c6-141">JSON Representation</span></span>
<span data-ttu-id="359c6-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="359c6-142">Here is a JSON representation of the resource.</span></span>
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




