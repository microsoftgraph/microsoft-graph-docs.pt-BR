---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bd7815b396f6a8ad79e9369eed72bbb9be23cfb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459704"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="9304c-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="9304c-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="9304c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9304c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9304c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9304c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9304c-106">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="9304c-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="9304c-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9304c-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9304c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9304c-108">Properties</span></span>
|<span data-ttu-id="9304c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9304c-109">Property</span></span>|<span data-ttu-id="9304c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9304c-110">Type</span></span>|<span data-ttu-id="9304c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9304c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9304c-112">actionName</span><span class="sxs-lookup"><span data-stu-id="9304c-112">actionName</span></span>|<span data-ttu-id="9304c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9304c-113">String</span></span>|<span data-ttu-id="9304c-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9304c-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9304c-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9304c-115">actionState</span></span>|[<span data-ttu-id="9304c-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9304c-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9304c-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9304c-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9304c-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9304c-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9304c-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9304c-119">startDateTime</span></span>|<span data-ttu-id="9304c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9304c-120">DateTimeOffset</span></span>|<span data-ttu-id="9304c-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9304c-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9304c-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9304c-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="9304c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9304c-123">DateTimeOffset</span></span>|<span data-ttu-id="9304c-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9304c-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9304c-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9304c-125">userPrincipalName</span></span>|<span data-ttu-id="9304c-126">String</span><span class="sxs-lookup"><span data-stu-id="9304c-126">String</span></span>|<span data-ttu-id="9304c-127">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="9304c-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="9304c-128">Relações</span><span class="sxs-lookup"><span data-stu-id="9304c-128">Relationships</span></span>
<span data-ttu-id="9304c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9304c-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9304c-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9304c-130">JSON Representation</span></span>
<span data-ttu-id="9304c-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9304c-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```







