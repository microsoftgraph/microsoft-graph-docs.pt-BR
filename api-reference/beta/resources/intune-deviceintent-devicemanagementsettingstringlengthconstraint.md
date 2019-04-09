---
title: tipo de recurso deviceManagementSettingStringLengthConstraint
description: Restrição que impõe um determinado intervalo de duração da cadeia de caracteres
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49d009571cdccf60dc8adcc2f1a703d39d0674c7
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522332"
---
# <a name="devicemanagementsettingstringlengthconstraint-resource-type"></a><span data-ttu-id="0cf9b-103">tipo de recurso deviceManagementSettingStringLengthConstraint</span><span class="sxs-lookup"><span data-stu-id="0cf9b-103">deviceManagementSettingStringLengthConstraint resource type</span></span>

> <span data-ttu-id="0cf9b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0cf9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cf9b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0cf9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cf9b-106">Restrição que impõe um determinado intervalo de duração da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf9b-106">Constraint enforcing a given string length range</span></span>


<span data-ttu-id="0cf9b-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="0cf9b-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0cf9b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cf9b-108">Properties</span></span>
|<span data-ttu-id="0cf9b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cf9b-109">Property</span></span>|<span data-ttu-id="0cf9b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cf9b-110">Type</span></span>|<span data-ttu-id="0cf9b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cf9b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cf9b-112">minimumLength</span><span class="sxs-lookup"><span data-stu-id="0cf9b-112">minimumLength</span></span>|<span data-ttu-id="0cf9b-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf9b-113">Int32</span></span>|<span data-ttu-id="0cf9b-114">O tamanho mínimo permitido da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf9b-114">The minimum permitted string length</span></span>|
|<span data-ttu-id="0cf9b-115">maximumLength</span><span class="sxs-lookup"><span data-stu-id="0cf9b-115">maximumLength</span></span>|<span data-ttu-id="0cf9b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf9b-116">Int32</span></span>|<span data-ttu-id="0cf9b-117">O tamanho máximo permitido da cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0cf9b-117">The maximum permitted string length</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cf9b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0cf9b-118">Relationships</span></span>
<span data-ttu-id="0cf9b-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0cf9b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cf9b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cf9b-120">JSON Representation</span></span>
<span data-ttu-id="0cf9b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cf9b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingStringLengthConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingStringLengthConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```







