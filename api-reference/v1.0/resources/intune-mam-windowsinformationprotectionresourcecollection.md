---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74d7549f57ecc59f70aa1af4350544ec21b156ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574457"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="5f111-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="5f111-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="5f111-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5f111-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f111-105">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="5f111-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="5f111-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f111-106">Properties</span></span>
|<span data-ttu-id="5f111-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f111-107">Property</span></span>|<span data-ttu-id="5f111-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f111-108">Type</span></span>|<span data-ttu-id="5f111-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f111-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f111-110">displayName</span><span class="sxs-lookup"><span data-stu-id="5f111-110">displayName</span></span>|<span data-ttu-id="5f111-111">String</span><span class="sxs-lookup"><span data-stu-id="5f111-111">String</span></span>|<span data-ttu-id="5f111-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="5f111-112">Display name</span></span>|
|<span data-ttu-id="5f111-113">recursos</span><span class="sxs-lookup"><span data-stu-id="5f111-113">resources</span></span>|<span data-ttu-id="5f111-114">String collection</span><span class="sxs-lookup"><span data-stu-id="5f111-114">String collection</span></span>|<span data-ttu-id="5f111-115">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="5f111-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f111-116">Relações</span><span class="sxs-lookup"><span data-stu-id="5f111-116">Relationships</span></span>
<span data-ttu-id="5f111-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f111-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f111-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f111-118">JSON Representation</span></span>
<span data-ttu-id="5f111-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f111-119">Here is a JSON representation of the resource.</span></span>
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



