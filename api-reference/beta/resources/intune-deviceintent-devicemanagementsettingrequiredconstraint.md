---
title: tipo de recurso deviceManagementSettingRequiredConstraint
description: Restrição que impõe uma determinada configuração necessária que não é nula/indefinida/sequência vazia/não configurada
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a077be2aac78b468ba7b265f8154ceee29803eef
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785285"
---
# <a name="devicemanagementsettingrequiredconstraint-resource-type"></a><span data-ttu-id="f2e19-103">tipo de recurso deviceManagementSettingRequiredConstraint</span><span class="sxs-lookup"><span data-stu-id="f2e19-103">deviceManagementSettingRequiredConstraint resource type</span></span>

> <span data-ttu-id="f2e19-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2e19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2e19-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2e19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2e19-106">Restrição que impõe uma determinada configuração necessária que não é nula/indefinida/sequência vazia/não configurada</span><span class="sxs-lookup"><span data-stu-id="f2e19-106">Constraint that enforces a particular required setting that is not null/undefined/empty string/not configured</span></span>


<span data-ttu-id="f2e19-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="f2e19-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2e19-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2e19-108">Properties</span></span>
|<span data-ttu-id="f2e19-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2e19-109">Property</span></span>|<span data-ttu-id="f2e19-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2e19-110">Type</span></span>|<span data-ttu-id="f2e19-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2e19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e19-112">Não configuravalue</span><span class="sxs-lookup"><span data-stu-id="f2e19-112">notConfiguredValue</span></span>|<span data-ttu-id="f2e19-113">String</span><span class="sxs-lookup"><span data-stu-id="f2e19-113">String</span></span>|<span data-ttu-id="f2e19-114">Lista de valores que significa não configurado para a configuração</span><span class="sxs-lookup"><span data-stu-id="f2e19-114">List of value which means not configured for the setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2e19-115">Relações</span><span class="sxs-lookup"><span data-stu-id="f2e19-115">Relationships</span></span>
<span data-ttu-id="f2e19-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2e19-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2e19-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2e19-117">JSON Representation</span></span>
<span data-ttu-id="f2e19-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2e19-118">Here is a JSON representation of the resource.</span></span>
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



