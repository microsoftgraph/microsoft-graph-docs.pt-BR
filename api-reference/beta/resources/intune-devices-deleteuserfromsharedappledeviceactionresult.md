---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e956edd96d752b50f189b951ac686deb78ba026d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968537"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="6a5fb-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="6a5fb-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="6a5fb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a5fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a5fb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a5fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a5fb-106">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="6a5fb-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="6a5fb-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a5fb-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a5fb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a5fb-108">Properties</span></span>
|<span data-ttu-id="6a5fb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a5fb-109">Property</span></span>|<span data-ttu-id="6a5fb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a5fb-110">Type</span></span>|<span data-ttu-id="6a5fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a5fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a5fb-112">actionName</span><span class="sxs-lookup"><span data-stu-id="6a5fb-112">actionName</span></span>|<span data-ttu-id="6a5fb-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a5fb-113">String</span></span>|<span data-ttu-id="6a5fb-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a5fb-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6a5fb-115">actionState</span><span class="sxs-lookup"><span data-stu-id="6a5fb-115">actionState</span></span>|[<span data-ttu-id="6a5fb-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6a5fb-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6a5fb-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6a5fb-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="6a5fb-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6a5fb-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6a5fb-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6a5fb-119">startDateTime</span></span>|<span data-ttu-id="6a5fb-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a5fb-120">DateTimeOffset</span></span>|<span data-ttu-id="6a5fb-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a5fb-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6a5fb-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a5fb-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="6a5fb-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a5fb-123">DateTimeOffset</span></span>|<span data-ttu-id="6a5fb-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6a5fb-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6a5fb-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a5fb-125">userPrincipalName</span></span>|<span data-ttu-id="6a5fb-126">String</span><span class="sxs-lookup"><span data-stu-id="6a5fb-126">String</span></span>|<span data-ttu-id="6a5fb-127">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="6a5fb-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a5fb-128">Relações</span><span class="sxs-lookup"><span data-stu-id="6a5fb-128">Relationships</span></span>
<span data-ttu-id="6a5fb-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a5fb-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a5fb-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a5fb-130">JSON Representation</span></span>
<span data-ttu-id="6a5fb-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a5fb-131">Here is a JSON representation of the resource.</span></span>
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





