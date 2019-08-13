---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 962a54ad2426be805e392db2f55a08985afe6b74
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370218"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="8da3b-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="8da3b-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="8da3b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8da3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8da3b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8da3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8da3b-106">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="8da3b-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="8da3b-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8da3b-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8da3b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8da3b-108">Properties</span></span>
|<span data-ttu-id="8da3b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8da3b-109">Property</span></span>|<span data-ttu-id="8da3b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8da3b-110">Type</span></span>|<span data-ttu-id="8da3b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8da3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8da3b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="8da3b-112">actionName</span></span>|<span data-ttu-id="8da3b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8da3b-113">String</span></span>|<span data-ttu-id="8da3b-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8da3b-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8da3b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8da3b-115">actionState</span></span>|[<span data-ttu-id="8da3b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="8da3b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="8da3b-117">Estado da ação herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="8da3b-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8da3b-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8da3b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8da3b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8da3b-119">startDateTime</span></span>|<span data-ttu-id="8da3b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8da3b-120">DateTimeOffset</span></span>|<span data-ttu-id="8da3b-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8da3b-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8da3b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8da3b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="8da3b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8da3b-123">DateTimeOffset</span></span>|<span data-ttu-id="8da3b-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8da3b-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8da3b-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8da3b-125">userPrincipalName</span></span>|<span data-ttu-id="8da3b-126">String</span><span class="sxs-lookup"><span data-stu-id="8da3b-126">String</span></span>|<span data-ttu-id="8da3b-127">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="8da3b-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="8da3b-128">Relações</span><span class="sxs-lookup"><span data-stu-id="8da3b-128">Relationships</span></span>
<span data-ttu-id="8da3b-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8da3b-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8da3b-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8da3b-130">JSON Representation</span></span>
<span data-ttu-id="8da3b-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8da3b-131">Here is a JSON representation of the resource.</span></span>
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



