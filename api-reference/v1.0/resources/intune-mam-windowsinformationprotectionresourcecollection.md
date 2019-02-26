---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74d7549f57ecc59f70aa1af4350544ec21b156ec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254818"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="20b22-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="20b22-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="20b22-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20b22-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20b22-105">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="20b22-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="20b22-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20b22-106">Properties</span></span>
|<span data-ttu-id="20b22-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20b22-107">Property</span></span>|<span data-ttu-id="20b22-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="20b22-108">Type</span></span>|<span data-ttu-id="20b22-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="20b22-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20b22-110">displayName</span><span class="sxs-lookup"><span data-stu-id="20b22-110">displayName</span></span>|<span data-ttu-id="20b22-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20b22-111">String</span></span>|<span data-ttu-id="20b22-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="20b22-112">Display name</span></span>|
|<span data-ttu-id="20b22-113">recursos</span><span class="sxs-lookup"><span data-stu-id="20b22-113">resources</span></span>|<span data-ttu-id="20b22-114">String collection</span><span class="sxs-lookup"><span data-stu-id="20b22-114">String collection</span></span>|<span data-ttu-id="20b22-115">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="20b22-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="20b22-116">Relações</span><span class="sxs-lookup"><span data-stu-id="20b22-116">Relationships</span></span>
<span data-ttu-id="20b22-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20b22-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20b22-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20b22-118">JSON Representation</span></span>
<span data-ttu-id="20b22-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20b22-119">Here is a JSON representation of the resource.</span></span>
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



