---
title: tipo de recurso deviceManagementSettingFileConstraint
description: A restrição que impõe a extensão do arquivo é aceitável para uma determinada configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60ff6a00e30e328daf2330e39511956ec1ab1f18
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924623"
---
# <a name="devicemanagementsettingfileconstraint-resource-type"></a><span data-ttu-id="7cb51-103">tipo de recurso deviceManagementSettingFileConstraint</span><span class="sxs-lookup"><span data-stu-id="7cb51-103">deviceManagementSettingFileConstraint resource type</span></span>

> <span data-ttu-id="7cb51-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7cb51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cb51-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7cb51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cb51-106">A restrição que impõe a extensão do arquivo é aceitável para uma determinada configuração</span><span class="sxs-lookup"><span data-stu-id="7cb51-106">Constraint enforcing the file extension is acceptable for a given setting</span></span>


<span data-ttu-id="7cb51-107">Herda de [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="7cb51-107">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7cb51-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7cb51-108">Properties</span></span>
|<span data-ttu-id="7cb51-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cb51-109">Property</span></span>|<span data-ttu-id="7cb51-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cb51-110">Type</span></span>|<span data-ttu-id="7cb51-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cb51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cb51-112">supportedExtensions</span><span class="sxs-lookup"><span data-stu-id="7cb51-112">supportedExtensions</span></span>|<span data-ttu-id="7cb51-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cb51-113">String collection</span></span>|<span data-ttu-id="7cb51-114">Extensões de arquivo aceitáveis para carregar essa configuração</span><span class="sxs-lookup"><span data-stu-id="7cb51-114">Acceptable file extensions to upload for this setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cb51-115">Relações</span><span class="sxs-lookup"><span data-stu-id="7cb51-115">Relationships</span></span>
<span data-ttu-id="7cb51-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7cb51-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cb51-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7cb51-117">JSON Representation</span></span>
<span data-ttu-id="7cb51-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7cb51-118">Here is a JSON representation of the resource.</span></span>
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



