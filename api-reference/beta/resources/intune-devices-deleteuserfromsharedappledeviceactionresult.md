---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d615aa333f184569ec3f1424a4aa154407c1ce8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060598"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="b6234-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="b6234-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="b6234-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6234-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6234-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6234-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6234-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6234-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6234-107">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="b6234-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="b6234-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b6234-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b6234-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6234-109">Properties</span></span>
|<span data-ttu-id="b6234-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6234-110">Property</span></span>|<span data-ttu-id="b6234-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6234-111">Type</span></span>|<span data-ttu-id="b6234-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6234-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6234-113">actionName</span><span class="sxs-lookup"><span data-stu-id="b6234-113">actionName</span></span>|<span data-ttu-id="b6234-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6234-114">String</span></span>|<span data-ttu-id="b6234-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b6234-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b6234-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b6234-116">actionState</span></span>|[<span data-ttu-id="b6234-117">actionState</span><span class="sxs-lookup"><span data-stu-id="b6234-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b6234-118">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b6234-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b6234-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b6234-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b6234-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b6234-120">startDateTime</span></span>|<span data-ttu-id="b6234-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6234-121">DateTimeOffset</span></span>|<span data-ttu-id="b6234-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b6234-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b6234-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6234-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="b6234-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6234-124">DateTimeOffset</span></span>|<span data-ttu-id="b6234-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b6234-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b6234-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6234-126">userPrincipalName</span></span>|<span data-ttu-id="b6234-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6234-127">String</span></span>|<span data-ttu-id="b6234-128">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="b6234-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6234-129">Relações</span><span class="sxs-lookup"><span data-stu-id="b6234-129">Relationships</span></span>
<span data-ttu-id="b6234-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6234-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6234-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6234-131">JSON Representation</span></span>
<span data-ttu-id="b6234-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6234-132">Here is a JSON representation of the resource.</span></span>
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






