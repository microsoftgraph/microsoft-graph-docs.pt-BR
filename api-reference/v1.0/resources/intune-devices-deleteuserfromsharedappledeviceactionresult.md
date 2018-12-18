---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: tfitzmac
ms.openlocfilehash: 2dc6dbdeb8bb72314b25f695f82e4f4dfff0b8fd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356032"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="9b5bf-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="9b5bf-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="9b5bf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9b5bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b5bf-105">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="9b5bf-105">Delete user from shared apple device action result</span></span>

<span data-ttu-id="9b5bf-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b5bf-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b5bf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b5bf-107">Properties</span></span>
|<span data-ttu-id="9b5bf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b5bf-108">Property</span></span>|<span data-ttu-id="9b5bf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b5bf-109">Type</span></span>|<span data-ttu-id="9b5bf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b5bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b5bf-111">actionName</span><span class="sxs-lookup"><span data-stu-id="9b5bf-111">actionName</span></span>|<span data-ttu-id="9b5bf-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b5bf-112">String</span></span>|<span data-ttu-id="9b5bf-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b5bf-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b5bf-114">actionState</span><span class="sxs-lookup"><span data-stu-id="9b5bf-114">actionState</span></span>|[<span data-ttu-id="9b5bf-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9b5bf-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9b5bf-116">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9b5bf-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9b5bf-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9b5bf-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9b5bf-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9b5bf-118">startDateTime</span></span>|<span data-ttu-id="9b5bf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b5bf-119">DateTimeOffset</span></span>|<span data-ttu-id="9b5bf-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b5bf-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b5bf-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b5bf-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="9b5bf-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b5bf-122">DateTimeOffset</span></span>|<span data-ttu-id="9b5bf-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b5bf-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b5bf-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9b5bf-124">userPrincipalName</span></span>|<span data-ttu-id="9b5bf-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b5bf-125">String</span></span>|<span data-ttu-id="9b5bf-126">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="9b5bf-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b5bf-127">Relações</span><span class="sxs-lookup"><span data-stu-id="9b5bf-127">Relationships</span></span>
<span data-ttu-id="9b5bf-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b5bf-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b5bf-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b5bf-129">JSON Representation</span></span>
<span data-ttu-id="9b5bf-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b5bf-130">Here is a JSON representation of the resource.</span></span>
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



