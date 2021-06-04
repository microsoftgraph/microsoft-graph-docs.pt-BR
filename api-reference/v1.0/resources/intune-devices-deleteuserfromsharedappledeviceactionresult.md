---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01680cd7604f1b830398fd77086b77d20028d7bc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754592"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="4e2a9-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="4e2a9-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="4e2a9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e2a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e2a9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4e2a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e2a9-106">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="4e2a9-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="4e2a9-107">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e2a9-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e2a9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e2a9-108">Properties</span></span>
|<span data-ttu-id="4e2a9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e2a9-109">Property</span></span>|<span data-ttu-id="4e2a9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e2a9-110">Type</span></span>|<span data-ttu-id="4e2a9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e2a9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e2a9-112">actionName</span><span class="sxs-lookup"><span data-stu-id="4e2a9-112">actionName</span></span>|<span data-ttu-id="4e2a9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e2a9-113">String</span></span>|<span data-ttu-id="4e2a9-114">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e2a9-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e2a9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="4e2a9-115">actionState</span></span>|[<span data-ttu-id="4e2a9-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4e2a9-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="4e2a9-117">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="4e2a9-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4e2a9-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4e2a9-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4e2a9-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4e2a9-119">startDateTime</span></span>|<span data-ttu-id="4e2a9-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e2a9-120">DateTimeOffset</span></span>|<span data-ttu-id="4e2a9-121">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e2a9-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e2a9-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e2a9-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="4e2a9-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e2a9-123">DateTimeOffset</span></span>|<span data-ttu-id="4e2a9-124">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4e2a9-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4e2a9-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e2a9-125">userPrincipalName</span></span>|<span data-ttu-id="4e2a9-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e2a9-126">String</span></span>|<span data-ttu-id="4e2a9-127">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="4e2a9-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e2a9-128">Relações</span><span class="sxs-lookup"><span data-stu-id="4e2a9-128">Relationships</span></span>
<span data-ttu-id="4e2a9-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4e2a9-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e2a9-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e2a9-130">JSON Representation</span></span>
<span data-ttu-id="4e2a9-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e2a9-131">Here is a JSON representation of the resource.</span></span>
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




