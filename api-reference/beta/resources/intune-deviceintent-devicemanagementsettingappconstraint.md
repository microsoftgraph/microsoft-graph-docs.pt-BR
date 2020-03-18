---
title: tipo de recurso deviceManagementSettingAppConstraint
description: A restrição que impõe a configuração contém somente tipos de aplicativos disponíveis.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b80fa581686692a47051405cc68f4d6d0694b95
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785376"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="5b009-103">tipo de recurso deviceManagementSettingAppConstraint</span><span class="sxs-lookup"><span data-stu-id="5b009-103">deviceManagementSettingAppConstraint resource type</span></span>

> <span data-ttu-id="5b009-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b009-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b009-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b009-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b009-106">A restrição que impõe a configuração contém somente tipos de aplicativos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="5b009-106">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="5b009-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="5b009-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b009-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b009-108">Properties</span></span>
|<span data-ttu-id="5b009-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b009-109">Property</span></span>|<span data-ttu-id="5b009-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b009-110">Type</span></span>|<span data-ttu-id="5b009-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b009-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b009-112">supportedTypes</span><span class="sxs-lookup"><span data-stu-id="5b009-112">supportedTypes</span></span>|<span data-ttu-id="5b009-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b009-113">String collection</span></span>|<span data-ttu-id="5b009-114">Tipos de aplicativos aceitáveis para permitir essa configuração</span><span class="sxs-lookup"><span data-stu-id="5b009-114">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b009-115">Relações</span><span class="sxs-lookup"><span data-stu-id="5b009-115">Relationships</span></span>
<span data-ttu-id="5b009-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b009-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b009-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b009-117">JSON Representation</span></span>
<span data-ttu-id="5b009-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b009-118">Here is a JSON representation of the resource.</span></span>
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



