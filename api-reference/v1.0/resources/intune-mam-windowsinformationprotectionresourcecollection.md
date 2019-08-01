---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 754f5ce902ca4cb5bb63be41f0e8094cc0738c26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037636"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="af4b1-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="af4b1-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="af4b1-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="af4b1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af4b1-105">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="af4b1-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="af4b1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af4b1-106">Properties</span></span>
|<span data-ttu-id="af4b1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af4b1-107">Property</span></span>|<span data-ttu-id="af4b1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="af4b1-108">Type</span></span>|<span data-ttu-id="af4b1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="af4b1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af4b1-110">displayName</span><span class="sxs-lookup"><span data-stu-id="af4b1-110">displayName</span></span>|<span data-ttu-id="af4b1-111">String</span><span class="sxs-lookup"><span data-stu-id="af4b1-111">String</span></span>|<span data-ttu-id="af4b1-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="af4b1-112">Display name</span></span>|
|<span data-ttu-id="af4b1-113">recursos</span><span class="sxs-lookup"><span data-stu-id="af4b1-113">resources</span></span>|<span data-ttu-id="af4b1-114">String collection</span><span class="sxs-lookup"><span data-stu-id="af4b1-114">String collection</span></span>|<span data-ttu-id="af4b1-115">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="af4b1-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="af4b1-116">Relações</span><span class="sxs-lookup"><span data-stu-id="af4b1-116">Relationships</span></span>
<span data-ttu-id="af4b1-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af4b1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af4b1-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af4b1-118">JSON Representation</span></span>
<span data-ttu-id="af4b1-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af4b1-119">Here is a JSON representation of the resource.</span></span>
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



