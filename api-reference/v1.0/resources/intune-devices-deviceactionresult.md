---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d08b4285f81c7b6f7e4962c4738279f84ba37b7d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541973"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="1cc9a-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="1cc9a-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="1cc9a-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cc9a-105">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="1cc9a-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="1cc9a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cc9a-106">Properties</span></span>
|<span data-ttu-id="1cc9a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cc9a-107">Property</span></span>|<span data-ttu-id="1cc9a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cc9a-108">Type</span></span>|<span data-ttu-id="1cc9a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc9a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cc9a-110">actionName</span><span class="sxs-lookup"><span data-stu-id="1cc9a-110">actionName</span></span>|<span data-ttu-id="1cc9a-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1cc9a-111">String</span></span>|<span data-ttu-id="1cc9a-112">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="1cc9a-112">Action name</span></span>|
|<span data-ttu-id="1cc9a-113">actionState</span><span class="sxs-lookup"><span data-stu-id="1cc9a-113">actionState</span></span>|[<span data-ttu-id="1cc9a-114">actionState</span><span class="sxs-lookup"><span data-stu-id="1cc9a-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="1cc9a-115">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-115">State of the action.</span></span> <span data-ttu-id="1cc9a-116">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1cc9a-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1cc9a-117">startDateTime</span></span>|<span data-ttu-id="1cc9a-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cc9a-118">DateTimeOffset</span></span>|<span data-ttu-id="1cc9a-119">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="1cc9a-119">Time the action was initiated</span></span>|
|<span data-ttu-id="1cc9a-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cc9a-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="1cc9a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cc9a-121">DateTimeOffset</span></span>|<span data-ttu-id="1cc9a-122">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="1cc9a-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cc9a-123">Relações</span><span class="sxs-lookup"><span data-stu-id="1cc9a-123">Relationships</span></span>
<span data-ttu-id="1cc9a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1cc9a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cc9a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cc9a-125">JSON Representation</span></span>
<span data-ttu-id="1cc9a-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cc9a-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



