---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1965a537726ebbaa0d461ea31403dd1110867f9a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533305"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="8ed88-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="8ed88-103">deviceActionResult resource type</span></span>

<span data-ttu-id="8ed88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ed88-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ed88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ed88-106">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="8ed88-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="8ed88-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ed88-107">Properties</span></span>
|<span data-ttu-id="8ed88-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ed88-108">Property</span></span>|<span data-ttu-id="8ed88-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ed88-109">Type</span></span>|<span data-ttu-id="8ed88-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ed88-111">actionName</span><span class="sxs-lookup"><span data-stu-id="8ed88-111">actionName</span></span>|<span data-ttu-id="8ed88-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8ed88-112">String</span></span>|<span data-ttu-id="8ed88-113">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="8ed88-113">Action name</span></span>|
|<span data-ttu-id="8ed88-114">actionState</span><span class="sxs-lookup"><span data-stu-id="8ed88-114">actionState</span></span>|[<span data-ttu-id="8ed88-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8ed88-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="8ed88-116">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="8ed88-116">State of the action.</span></span> <span data-ttu-id="8ed88-117">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8ed88-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8ed88-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed88-118">startDateTime</span></span>|<span data-ttu-id="8ed88-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ed88-119">DateTimeOffset</span></span>|<span data-ttu-id="8ed88-120">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="8ed88-120">Time the action was initiated</span></span>|
|<span data-ttu-id="8ed88-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed88-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="8ed88-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ed88-122">DateTimeOffset</span></span>|<span data-ttu-id="8ed88-123">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="8ed88-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ed88-124">Relações</span><span class="sxs-lookup"><span data-stu-id="8ed88-124">Relationships</span></span>
<span data-ttu-id="8ed88-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8ed88-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ed88-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ed88-126">JSON Representation</span></span>
<span data-ttu-id="8ed88-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ed88-127">Here is a JSON representation of the resource.</span></span>
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




