---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c6e014f0461c1e6a72a4d67791c27dc401f87f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804946"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="5a228-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="5a228-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="5a228-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5a228-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a228-105">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="5a228-105">Delete user from shared apple device action result</span></span>

<span data-ttu-id="5a228-106">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5a228-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5a228-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a228-107">Properties</span></span>
|<span data-ttu-id="5a228-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a228-108">Property</span></span>|<span data-ttu-id="5a228-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a228-109">Type</span></span>|<span data-ttu-id="5a228-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a228-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a228-111">actionName</span><span class="sxs-lookup"><span data-stu-id="5a228-111">actionName</span></span>|<span data-ttu-id="5a228-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a228-112">String</span></span>|<span data-ttu-id="5a228-113">Nome da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5a228-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5a228-114">actionState</span><span class="sxs-lookup"><span data-stu-id="5a228-114">actionState</span></span>|[<span data-ttu-id="5a228-115">actionState</span><span class="sxs-lookup"><span data-stu-id="5a228-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="5a228-116">Estado da ação Inherited de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="5a228-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="5a228-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5a228-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5a228-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5a228-118">startDateTime</span></span>|<span data-ttu-id="5a228-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a228-119">DateTimeOffset</span></span>|<span data-ttu-id="5a228-120">Hora em que ação foi iniciada, herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5a228-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5a228-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a228-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="5a228-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a228-122">DateTimeOffset</span></span>|<span data-ttu-id="5a228-123">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="5a228-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="5a228-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5a228-124">userPrincipalName</span></span>|<span data-ttu-id="5a228-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a228-125">String</span></span>|<span data-ttu-id="5a228-126">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="5a228-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a228-127">Relações</span><span class="sxs-lookup"><span data-stu-id="5a228-127">Relationships</span></span>
<span data-ttu-id="5a228-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a228-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a228-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a228-129">JSON Representation</span></span>
<span data-ttu-id="5a228-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a228-130">Here is a JSON representation of the resource.</span></span>
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



