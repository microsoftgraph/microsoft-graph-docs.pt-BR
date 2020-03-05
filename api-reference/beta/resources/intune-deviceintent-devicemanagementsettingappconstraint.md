---
title: tipo de recurso deviceManagementSettingAppConstraint
description: A restrição que impõe a configuração contém somente tipos de aplicativos disponíveis.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7818493bb5767ce74d0f6f71cf5ffa05a775eded
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525275"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="e0db0-103">tipo de recurso deviceManagementSettingAppConstraint</span><span class="sxs-lookup"><span data-stu-id="e0db0-103">deviceManagementSettingAppConstraint resource type</span></span>

<span data-ttu-id="e0db0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e0db0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0db0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e0db0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0db0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e0db0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0db0-107">A restrição que impõe a configuração contém somente tipos de aplicativos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="e0db0-107">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="e0db0-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e0db0-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0db0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0db0-109">Properties</span></span>
|<span data-ttu-id="e0db0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0db0-110">Property</span></span>|<span data-ttu-id="e0db0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0db0-111">Type</span></span>|<span data-ttu-id="e0db0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0db0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0db0-113">supportedTypes</span><span class="sxs-lookup"><span data-stu-id="e0db0-113">supportedTypes</span></span>|<span data-ttu-id="e0db0-114">String collection</span><span class="sxs-lookup"><span data-stu-id="e0db0-114">String collection</span></span>|<span data-ttu-id="e0db0-115">Tipos de aplicativos aceitáveis para permitir essa configuração</span><span class="sxs-lookup"><span data-stu-id="e0db0-115">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0db0-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e0db0-116">Relationships</span></span>
<span data-ttu-id="e0db0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0db0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0db0-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0db0-118">JSON Representation</span></span>
<span data-ttu-id="e0db0-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0db0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingAppConstraint",
  "supportedTypes": [
    "String"
  ]
}
```



