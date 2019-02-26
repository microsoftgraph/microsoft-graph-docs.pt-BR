---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5071c0c9168cfedbbaa527f82241c80b4ad53705
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261520"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="81a26-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="81a26-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="81a26-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81a26-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a26-105">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="81a26-105">Delete user from shared apple device action result</span></span>


<span data-ttu-id="81a26-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="81a26-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81a26-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81a26-107">Properties</span></span>
|<span data-ttu-id="81a26-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81a26-108">Property</span></span>|<span data-ttu-id="81a26-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="81a26-109">Type</span></span>|<span data-ttu-id="81a26-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81a26-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a26-111">actionName</span><span class="sxs-lookup"><span data-stu-id="81a26-111">actionName</span></span>|<span data-ttu-id="81a26-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81a26-112">String</span></span>|<span data-ttu-id="81a26-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="81a26-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="81a26-114">actionState</span><span class="sxs-lookup"><span data-stu-id="81a26-114">actionState</span></span>|[<span data-ttu-id="81a26-115">actionState</span><span class="sxs-lookup"><span data-stu-id="81a26-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="81a26-116">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="81a26-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="81a26-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="81a26-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="81a26-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="81a26-118">startDateTime</span></span>|<span data-ttu-id="81a26-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a26-119">DateTimeOffset</span></span>|<span data-ttu-id="81a26-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="81a26-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="81a26-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="81a26-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="81a26-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81a26-122">DateTimeOffset</span></span>|<span data-ttu-id="81a26-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="81a26-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="81a26-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="81a26-124">userPrincipalName</span></span>|<span data-ttu-id="81a26-125">String</span><span class="sxs-lookup"><span data-stu-id="81a26-125">String</span></span>|<span data-ttu-id="81a26-126">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="81a26-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="81a26-127">Relações</span><span class="sxs-lookup"><span data-stu-id="81a26-127">Relationships</span></span>
<span data-ttu-id="81a26-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81a26-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81a26-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81a26-129">JSON Representation</span></span>
<span data-ttu-id="81a26-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81a26-130">Here is a JSON representation of the resource.</span></span>
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



