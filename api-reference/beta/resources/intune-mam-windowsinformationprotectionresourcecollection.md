---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbeb58464ccfd7aff3dfc6066ab276a2bd73f5c6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149746"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="c5030-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="c5030-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="c5030-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5030-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5030-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5030-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5030-106">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="c5030-106">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="c5030-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5030-107">Properties</span></span>
|<span data-ttu-id="c5030-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5030-108">Property</span></span>|<span data-ttu-id="c5030-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5030-109">Type</span></span>|<span data-ttu-id="c5030-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5030-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5030-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c5030-111">displayName</span></span>|<span data-ttu-id="c5030-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5030-112">String</span></span>|<span data-ttu-id="c5030-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="c5030-113">Display name</span></span>|
|<span data-ttu-id="c5030-114">recursos</span><span class="sxs-lookup"><span data-stu-id="c5030-114">resources</span></span>|<span data-ttu-id="c5030-115">String collection</span><span class="sxs-lookup"><span data-stu-id="c5030-115">String collection</span></span>|<span data-ttu-id="c5030-116">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="c5030-116">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5030-117">Relações</span><span class="sxs-lookup"><span data-stu-id="c5030-117">Relationships</span></span>
<span data-ttu-id="c5030-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5030-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5030-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5030-119">JSON Representation</span></span>
<span data-ttu-id="c5030-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5030-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




