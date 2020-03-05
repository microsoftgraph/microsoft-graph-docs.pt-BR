---
title: tipo de recurso deviceManagementSettingCollectionConstraint
description: Restrição que impõe o número máximo de elementos de uma coleção
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c285a7cff806585cc9e54b05011c22f8b385036f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528805"
---
# <a name="devicemanagementsettingcollectionconstraint-resource-type"></a><span data-ttu-id="ab108-103">tipo de recurso deviceManagementSettingCollectionConstraint</span><span class="sxs-lookup"><span data-stu-id="ab108-103">deviceManagementSettingCollectionConstraint resource type</span></span>

<span data-ttu-id="ab108-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ab108-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab108-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ab108-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab108-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab108-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab108-107">Restrição que impõe o número máximo de elementos de uma coleção</span><span class="sxs-lookup"><span data-stu-id="ab108-107">Constraint that enforces the maximum number of elements a collection</span></span>


<span data-ttu-id="ab108-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="ab108-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ab108-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab108-109">Properties</span></span>
|<span data-ttu-id="ab108-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab108-110">Property</span></span>|<span data-ttu-id="ab108-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab108-111">Type</span></span>|<span data-ttu-id="ab108-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab108-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab108-113">minimumLength</span><span class="sxs-lookup"><span data-stu-id="ab108-113">minimumLength</span></span>|<span data-ttu-id="ab108-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ab108-114">Int32</span></span>|<span data-ttu-id="ab108-115">O número mínimo de elementos na coleção</span><span class="sxs-lookup"><span data-stu-id="ab108-115">The minimum number of elements in the collection</span></span>|
|<span data-ttu-id="ab108-116">maximumLength</span><span class="sxs-lookup"><span data-stu-id="ab108-116">maximumLength</span></span>|<span data-ttu-id="ab108-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ab108-117">Int32</span></span>|<span data-ttu-id="ab108-118">O número máximo de elementos na coleção</span><span class="sxs-lookup"><span data-stu-id="ab108-118">The maximum number of elements in the collection</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab108-119">Relações</span><span class="sxs-lookup"><span data-stu-id="ab108-119">Relationships</span></span>
<span data-ttu-id="ab108-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ab108-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab108-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab108-121">JSON Representation</span></span>
<span data-ttu-id="ab108-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab108-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingCollectionConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCollectionConstraint",
  "minimumLength": 1024,
  "maximumLength": 1024
}
```



