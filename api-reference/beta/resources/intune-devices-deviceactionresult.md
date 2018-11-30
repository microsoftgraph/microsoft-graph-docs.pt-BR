---
title: Tipo de recurso deviceActionResult
description: Resultado de ação de dispositivo
ms.openlocfilehash: ac37cdff8ec323dfb8a2019b383d506c1b7e1076
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034405"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="3aca7-103">Tipo de recurso deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="3aca7-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="3aca7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3aca7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3aca7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3aca7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3aca7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3aca7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3aca7-107">Resultado de ação de dispositivo</span><span class="sxs-lookup"><span data-stu-id="3aca7-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="3aca7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3aca7-108">Properties</span></span>
|<span data-ttu-id="3aca7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3aca7-109">Property</span></span>|<span data-ttu-id="3aca7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3aca7-110">Type</span></span>|<span data-ttu-id="3aca7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3aca7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aca7-112">actionName</span><span class="sxs-lookup"><span data-stu-id="3aca7-112">actionName</span></span>|<span data-ttu-id="3aca7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3aca7-113">String</span></span>|<span data-ttu-id="3aca7-114">Nome da ação</span><span class="sxs-lookup"><span data-stu-id="3aca7-114">Action name</span></span>|
|<span data-ttu-id="3aca7-115">actionState</span><span class="sxs-lookup"><span data-stu-id="3aca7-115">actionState</span></span>|[<span data-ttu-id="3aca7-116">actionState</span><span class="sxs-lookup"><span data-stu-id="3aca7-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="3aca7-117">Estado da ação.</span><span class="sxs-lookup"><span data-stu-id="3aca7-117">State of the action.</span></span> <span data-ttu-id="3aca7-118">Os valores possíveis são: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3aca7-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3aca7-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3aca7-119">startDateTime</span></span>|<span data-ttu-id="3aca7-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aca7-120">DateTimeOffset</span></span>|<span data-ttu-id="3aca7-121">Hora em que a ação foi iniciada</span><span class="sxs-lookup"><span data-stu-id="3aca7-121">Time the action was initiated</span></span>|
|<span data-ttu-id="3aca7-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3aca7-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="3aca7-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aca7-123">DateTimeOffset</span></span>|<span data-ttu-id="3aca7-124">Hora da última atualização do estado da ação</span><span class="sxs-lookup"><span data-stu-id="3aca7-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="3aca7-125">Relações</span><span class="sxs-lookup"><span data-stu-id="3aca7-125">Relationships</span></span>
<span data-ttu-id="3aca7-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3aca7-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3aca7-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3aca7-127">JSON Representation</span></span>
<span data-ttu-id="3aca7-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3aca7-128">Here is a JSON representation of the resource.</span></span>
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





