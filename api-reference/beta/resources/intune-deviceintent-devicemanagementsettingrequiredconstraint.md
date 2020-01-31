---
title: tipo de recurso deviceManagementSettingRequiredConstraint
description: Restrição que impõe uma determinada configuração necessária que não é nula/indefinida/sequência vazia/não configurada
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b2df645780cdd7d06847d3acb18766027bf4ad8
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636599"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="d7f69-103">tipo de recurso deviceManagementSettingRequiredConstraint</span><span class="sxs-lookup"><span data-stu-id="d7f69-103">deviceManagementSettingRequiredConstraint resource type</span></span>

> <span data-ttu-id="d7f69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d7f69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7f69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d7f69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7f69-106">Restrição que impõe uma determinada configuração necessária que não é nula/indefinida/sequência vazia/não configurada</span><span class="sxs-lookup"><span data-stu-id="d7f69-106">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="d7f69-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="d7f69-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7f69-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7f69-108">Properties</span></span>
|<span data-ttu-id="d7f69-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7f69-109">Property</span></span>|<span data-ttu-id="d7f69-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7f69-110">Type</span></span>|<span data-ttu-id="d7f69-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7f69-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7f69-112">Não configuravalue</span><span class="sxs-lookup"><span data-stu-id="d7f69-112">notConfiguredValue</span></span>|<span data-ttu-id="d7f69-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7f69-113">String</span></span>|<span data-ttu-id="d7f69-114">Lista de valores que significa não configurado para a configuração</span><span class="sxs-lookup"><span data-stu-id="d7f69-114">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7f69-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d7f69-115">Relationships</span></span>
<span data-ttu-id="d7f69-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7f69-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7f69-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7f69-117">JSON Representation</span></span>
<span data-ttu-id="d7f69-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7f69-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingRequiredConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingRequiredConstraint",
  "notConfiguredValue": "String"
}
```



