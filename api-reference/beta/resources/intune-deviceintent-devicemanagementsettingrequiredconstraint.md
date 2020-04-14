---
title: tipo de recurso deviceManagementSettingRequiredConstraint
description: Restrição que impõe uma determinada configuração necessária que não é nula/indefinida/sequência vazia/não configurada
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd70066465fcde31ba12ff1a7deb96a41a6786e9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420082"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="3d9e4-103">tipo de recurso deviceManagementSettingRequiredConstraint</span><span class="sxs-lookup"><span data-stu-id="3d9e4-103">deviceManagementSettingRequiredConstraint resource type</span></span>

<span data-ttu-id="3d9e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d9e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d9e4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d9e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d9e4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d9e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d9e4-107">Restrição que impõe uma determinada configuração necessária que não é nula/indefinida/sequência vazia/não configurada</span><span class="sxs-lookup"><span data-stu-id="3d9e4-107">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="3d9e4-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="3d9e4-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3d9e4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d9e4-109">Properties</span></span>
|<span data-ttu-id="3d9e4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d9e4-110">Property</span></span>|<span data-ttu-id="3d9e4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d9e4-111">Type</span></span>|<span data-ttu-id="3d9e4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d9e4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d9e4-113">Não configuravalue</span><span class="sxs-lookup"><span data-stu-id="3d9e4-113">notConfiguredValue</span></span>|<span data-ttu-id="3d9e4-114">String</span><span class="sxs-lookup"><span data-stu-id="3d9e4-114">String</span></span>|<span data-ttu-id="3d9e4-115">Lista de valores que significa não configurado para a configuração</span><span class="sxs-lookup"><span data-stu-id="3d9e4-115">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d9e4-116">Relações</span><span class="sxs-lookup"><span data-stu-id="3d9e4-116">Relationships</span></span>
<span data-ttu-id="3d9e4-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d9e4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d9e4-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d9e4-118">JSON Representation</span></span>
<span data-ttu-id="3d9e4-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d9e4-119">Here is a JSON representation of the resource.</span></span>
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



