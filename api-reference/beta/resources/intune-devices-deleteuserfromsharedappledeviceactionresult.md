---
title: Tipo de recurso deleteUserFromSharedAppleDeviceActionResult
description: Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ca29d440f5721e16d13bf91dd366fb9e893108d
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610960"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="97a81-103">Tipo de recurso deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="97a81-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="97a81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97a81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97a81-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97a81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97a81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97a81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97a81-107">Resultado de ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="97a81-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="97a81-108">Herda de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="97a81-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97a81-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97a81-109">Properties</span></span>
|<span data-ttu-id="97a81-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97a81-110">Property</span></span>|<span data-ttu-id="97a81-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="97a81-111">Type</span></span>|<span data-ttu-id="97a81-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="97a81-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97a81-113">actionName</span><span class="sxs-lookup"><span data-stu-id="97a81-113">actionName</span></span>|<span data-ttu-id="97a81-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97a81-114">String</span></span>|<span data-ttu-id="97a81-115">Nome da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="97a81-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="97a81-116">actionState</span><span class="sxs-lookup"><span data-stu-id="97a81-116">actionState</span></span>|[<span data-ttu-id="97a81-117">actionState</span><span class="sxs-lookup"><span data-stu-id="97a81-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="97a81-118">Estado da ação Herdado de [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="97a81-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="97a81-119">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="97a81-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="97a81-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="97a81-120">startDateTime</span></span>|<span data-ttu-id="97a81-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97a81-121">DateTimeOffset</span></span>|<span data-ttu-id="97a81-122">Hora de início da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="97a81-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="97a81-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="97a81-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="97a81-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97a81-124">DateTimeOffset</span></span>|<span data-ttu-id="97a81-125">Hora da última atualização do estado da ação Herdada de [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="97a81-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="97a81-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97a81-126">userPrincipalName</span></span>|<span data-ttu-id="97a81-127">String</span><span class="sxs-lookup"><span data-stu-id="97a81-127">String</span></span>|<span data-ttu-id="97a81-128">Nome da entidade de segurança do usuário a ser excluído</span><span class="sxs-lookup"><span data-stu-id="97a81-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="97a81-129">Relações</span><span class="sxs-lookup"><span data-stu-id="97a81-129">Relationships</span></span>
<span data-ttu-id="97a81-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97a81-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97a81-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97a81-131">JSON Representation</span></span>
<span data-ttu-id="97a81-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97a81-132">Here is a JSON representation of the resource.</span></span>
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




