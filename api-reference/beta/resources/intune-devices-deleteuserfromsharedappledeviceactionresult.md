---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8206383e33ff0fa7a682485fe63d1ec978aa9e68
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456882"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="1aacb-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="1aacb-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="1aacb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1aacb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1aacb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1aacb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aacb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1aacb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aacb-107">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="1aacb-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="1aacb-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1aacb-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1aacb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1aacb-109">Properties</span></span>
|<span data-ttu-id="1aacb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1aacb-110">Property</span></span>|<span data-ttu-id="1aacb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aacb-111">Type</span></span>|<span data-ttu-id="1aacb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aacb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aacb-113">actionName</span><span class="sxs-lookup"><span data-stu-id="1aacb-113">actionName</span></span>|<span data-ttu-id="1aacb-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1aacb-114">String</span></span>|<span data-ttu-id="1aacb-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1aacb-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1aacb-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1aacb-116">actionState</span></span>|[<span data-ttu-id="1aacb-117">actionState</span><span class="sxs-lookup"><span data-stu-id="1aacb-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1aacb-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="1aacb-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="1aacb-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1aacb-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1aacb-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1aacb-120">startDateTime</span></span>|<span data-ttu-id="1aacb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aacb-121">DateTimeOffset</span></span>|<span data-ttu-id="1aacb-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1aacb-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1aacb-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1aacb-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="1aacb-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aacb-124">DateTimeOffset</span></span>|<span data-ttu-id="1aacb-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1aacb-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="1aacb-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1aacb-126">userPrincipalName</span></span>|<span data-ttu-id="1aacb-127">String</span><span class="sxs-lookup"><span data-stu-id="1aacb-127">String</span></span>|<span data-ttu-id="1aacb-128">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="1aacb-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aacb-129">Relações</span><span class="sxs-lookup"><span data-stu-id="1aacb-129">Relationships</span></span>
<span data-ttu-id="1aacb-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1aacb-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1aacb-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1aacb-131">JSON Representation</span></span>
<span data-ttu-id="1aacb-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1aacb-132">Here is a JSON representation of the resource.</span></span>
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



