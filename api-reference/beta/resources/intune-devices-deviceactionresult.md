---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 518d0d09d7ef4f9fea67ce8d600f97be0345fa63
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404705"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="9a920-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="9a920-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="9a920-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a920-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a920-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a920-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a920-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9a920-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a920-107">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="9a920-107">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="9a920-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a920-108">Properties</span></span>
|<span data-ttu-id="9a920-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a920-109">Property</span></span>|<span data-ttu-id="9a920-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a920-110">Type</span></span>|<span data-ttu-id="9a920-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a920-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a920-112">actionName</span><span class="sxs-lookup"><span data-stu-id="9a920-112">actionName</span></span>|<span data-ttu-id="9a920-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a920-113">String</span></span>|<span data-ttu-id="9a920-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="9a920-114">Action name</span></span>|
|<span data-ttu-id="9a920-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9a920-115">actionState</span></span>|[<span data-ttu-id="9a920-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9a920-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9a920-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="9a920-117">State of the action.</span></span> <span data-ttu-id="9a920-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9a920-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9a920-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9a920-119">startDateTime</span></span>|<span data-ttu-id="9a920-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a920-120">DateTimeOffset</span></span>|<span data-ttu-id="9a920-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="9a920-121">Time the action was initiated</span></span>|
|<span data-ttu-id="9a920-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a920-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="9a920-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a920-123">DateTimeOffset</span></span>|<span data-ttu-id="9a920-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="9a920-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a920-125">Relações</span><span class="sxs-lookup"><span data-stu-id="9a920-125">Relationships</span></span>
<span data-ttu-id="9a920-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a920-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a920-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a920-127">JSON Representation</span></span>
<span data-ttu-id="9a920-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a920-128">Here is a JSON representation of the resource.</span></span>
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




