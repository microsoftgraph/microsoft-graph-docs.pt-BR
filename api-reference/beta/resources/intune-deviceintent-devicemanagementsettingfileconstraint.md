---
title: tipo de recurso deviceManagementSettingFileConstraint
description: A restrição que impõe a extensão do arquivo é aceitável para uma determinada configuração
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9a9e5a3f4ce8cec54dbdd0f1a690b039b2da0524
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785320"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="4af54-103">tipo de recurso deviceManagementSettingFileConstraint</span><span class="sxs-lookup"><span data-stu-id="4af54-103">deviceManagementSettingFileConstraint resource type</span></span>

> <span data-ttu-id="4af54-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4af54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4af54-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4af54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4af54-106">A restrição que impõe a extensão do arquivo é aceitável para uma determinada configuração</span><span class="sxs-lookup"><span data-stu-id="4af54-106">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="4af54-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="4af54-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4af54-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4af54-108">Properties</span></span>
|<span data-ttu-id="4af54-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4af54-109">Property</span></span>|<span data-ttu-id="4af54-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4af54-110">Type</span></span>|<span data-ttu-id="4af54-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4af54-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4af54-112">supportedExtensions</span><span class="sxs-lookup"><span data-stu-id="4af54-112">supportedExtensions</span></span>|<span data-ttu-id="4af54-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4af54-113">String collection</span></span>|<span data-ttu-id="4af54-114">Extensões de arquivo aceitáveis para carregar essa configuração</span><span class="sxs-lookup"><span data-stu-id="4af54-114">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="4af54-115">Relações</span><span class="sxs-lookup"><span data-stu-id="4af54-115">Relationships</span></span>
<span data-ttu-id="4af54-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4af54-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4af54-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4af54-117">JSON Representation</span></span>
<span data-ttu-id="4af54-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4af54-118">Here is a JSON representation of the resource.</span></span>
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



