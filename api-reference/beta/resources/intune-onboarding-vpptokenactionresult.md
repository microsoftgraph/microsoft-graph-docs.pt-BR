---
title: tipo de recurso de vppTokenActionResult
description: O status da ação executada com um token de programa de compra de Volume do Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f3aa2467d8f30c023a7564817a2da9e1c970125f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961915"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="79bb5-103">tipo de recurso de vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="79bb5-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="79bb5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="79bb5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79bb5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="79bb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79bb5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="79bb5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79bb5-107">O status da ação executada com um token de programa de compra de Volume do Apple.</span><span class="sxs-lookup"><span data-stu-id="79bb5-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>
## <a name="properties"></a><span data-ttu-id="79bb5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79bb5-108">Properties</span></span>
|<span data-ttu-id="79bb5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79bb5-109">Property</span></span>|<span data-ttu-id="79bb5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="79bb5-110">Type</span></span>|<span data-ttu-id="79bb5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="79bb5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79bb5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="79bb5-112">actionName</span></span>|<span data-ttu-id="79bb5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79bb5-113">String</span></span>|<span data-ttu-id="79bb5-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="79bb5-114">Action name</span></span>|
|<span data-ttu-id="79bb5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="79bb5-115">actionState</span></span>|[<span data-ttu-id="79bb5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="79bb5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="79bb5-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="79bb5-117">State of the action.</span></span> <span data-ttu-id="79bb5-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="79bb5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="79bb5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="79bb5-119">startDateTime</span></span>|<span data-ttu-id="79bb5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79bb5-120">DateTimeOffset</span></span>|<span data-ttu-id="79bb5-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="79bb5-121">Time the action was initiated</span></span>|
|<span data-ttu-id="79bb5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="79bb5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="79bb5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79bb5-123">DateTimeOffset</span></span>|<span data-ttu-id="79bb5-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="79bb5-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="79bb5-125">Relações</span><span class="sxs-lookup"><span data-stu-id="79bb5-125">Relationships</span></span>
<span data-ttu-id="79bb5-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79bb5-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79bb5-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79bb5-127">JSON Representation</span></span>
<span data-ttu-id="79bb5-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79bb5-128">Here is a JSON representation of the resource.</span></span>
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





