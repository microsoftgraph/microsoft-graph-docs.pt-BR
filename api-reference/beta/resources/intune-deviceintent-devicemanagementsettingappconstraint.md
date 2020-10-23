---
title: tipo de recurso deviceManagementSettingAppConstraint
description: A restrição que impõe a configuração contém somente tipos de aplicativos disponíveis.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 891b7ed26b254bee7d52c732318e16ef0885904b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728290"
---
# <a name="devicemanagementsettingappconstraint-resource-type"></a><span data-ttu-id="a59b8-103">tipo de recurso deviceManagementSettingAppConstraint</span><span class="sxs-lookup"><span data-stu-id="a59b8-103">deviceManagementSettingAppConstraint resource type</span></span>

<span data-ttu-id="a59b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a59b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a59b8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a59b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a59b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a59b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a59b8-107">A restrição que impõe a configuração contém somente tipos de aplicativos disponíveis.</span><span class="sxs-lookup"><span data-stu-id="a59b8-107">Constraint enforcing the setting contains only vaild app types.</span></span>


<span data-ttu-id="a59b8-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="a59b8-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a59b8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a59b8-109">Properties</span></span>
|<span data-ttu-id="a59b8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a59b8-110">Property</span></span>|<span data-ttu-id="a59b8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a59b8-111">Type</span></span>|<span data-ttu-id="a59b8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a59b8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a59b8-113">supportedTypes</span><span class="sxs-lookup"><span data-stu-id="a59b8-113">supportedTypes</span></span>|<span data-ttu-id="a59b8-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a59b8-114">String collection</span></span>|<span data-ttu-id="a59b8-115">Tipos de aplicativos aceitáveis para permitir essa configuração</span><span class="sxs-lookup"><span data-stu-id="a59b8-115">Acceptable app types to allow for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="a59b8-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a59b8-116">Relationships</span></span>
<span data-ttu-id="a59b8-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a59b8-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a59b8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a59b8-118">JSON Representation</span></span>
<span data-ttu-id="a59b8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a59b8-119">Here is a JSON representation of the resource.</span></span>
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





