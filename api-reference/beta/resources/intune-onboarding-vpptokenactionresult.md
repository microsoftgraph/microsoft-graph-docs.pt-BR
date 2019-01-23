---
title: tipo de recurso de vppTokenActionResult
description: O status da ação executada com um token de programa de compra de Volume do Apple.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2fb78ea991ed43bd100a424ea7ddd7e23b22412d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414288"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="2b83a-103">tipo de recurso de vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="2b83a-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="2b83a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b83a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b83a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b83a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b83a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2b83a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b83a-107">O status da ação executada com um token de programa de compra de Volume do Apple.</span><span class="sxs-lookup"><span data-stu-id="2b83a-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="2b83a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b83a-108">Properties</span></span>
|<span data-ttu-id="2b83a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b83a-109">Property</span></span>|<span data-ttu-id="2b83a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b83a-110">Type</span></span>|<span data-ttu-id="2b83a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b83a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b83a-112">actionName</span><span class="sxs-lookup"><span data-stu-id="2b83a-112">actionName</span></span>|<span data-ttu-id="2b83a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b83a-113">String</span></span>|<span data-ttu-id="2b83a-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="2b83a-114">Action name</span></span>|
|<span data-ttu-id="2b83a-115">actionState</span><span class="sxs-lookup"><span data-stu-id="2b83a-115">actionState</span></span>|[<span data-ttu-id="2b83a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2b83a-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2b83a-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="2b83a-117">State of the action.</span></span> <span data-ttu-id="2b83a-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2b83a-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2b83a-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2b83a-119">startDateTime</span></span>|<span data-ttu-id="2b83a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b83a-120">DateTimeOffset</span></span>|<span data-ttu-id="2b83a-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="2b83a-121">Time the action was initiated</span></span>|
|<span data-ttu-id="2b83a-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b83a-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="2b83a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b83a-123">DateTimeOffset</span></span>|<span data-ttu-id="2b83a-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="2b83a-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b83a-125">Relações</span><span class="sxs-lookup"><span data-stu-id="2b83a-125">Relationships</span></span>
<span data-ttu-id="2b83a-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b83a-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b83a-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b83a-127">JSON Representation</span></span>
<span data-ttu-id="2b83a-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b83a-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




