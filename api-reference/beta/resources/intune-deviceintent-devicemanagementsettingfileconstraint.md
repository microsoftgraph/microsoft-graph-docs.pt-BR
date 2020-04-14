---
title: tipo de recurso deviceManagementSettingFileConstraint
description: A restrição que impõe a extensão do arquivo é aceitável para uma determinada configuração
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6864d70c31096147a51ff4b3e67a7053d93ed27b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443243"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="bf4f9-103">tipo de recurso deviceManagementSettingFileConstraint</span><span class="sxs-lookup"><span data-stu-id="bf4f9-103">deviceManagementSettingFileConstraint resource type</span></span>

<span data-ttu-id="bf4f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf4f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf4f9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bf4f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf4f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf4f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf4f9-107">A restrição que impõe a extensão do arquivo é aceitável para uma determinada configuração</span><span class="sxs-lookup"><span data-stu-id="bf4f9-107">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="bf4f9-108">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="bf4f9-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf4f9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf4f9-109">Properties</span></span>
|<span data-ttu-id="bf4f9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf4f9-110">Property</span></span>|<span data-ttu-id="bf4f9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf4f9-111">Type</span></span>|<span data-ttu-id="bf4f9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf4f9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf4f9-113">supportedExtensions</span><span class="sxs-lookup"><span data-stu-id="bf4f9-113">supportedExtensions</span></span>|<span data-ttu-id="bf4f9-114">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bf4f9-114">String collection</span></span>|<span data-ttu-id="bf4f9-115">Extensões de arquivo aceitáveis para carregar essa configuração</span><span class="sxs-lookup"><span data-stu-id="bf4f9-115">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf4f9-116">Relações</span><span class="sxs-lookup"><span data-stu-id="bf4f9-116">Relationships</span></span>
<span data-ttu-id="bf4f9-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf4f9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf4f9-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf4f9-118">JSON Representation</span></span>
<span data-ttu-id="bf4f9-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf4f9-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingFileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingFileConstraint",
  "supportedExtensions": [
    "String"
  ]
}
```



