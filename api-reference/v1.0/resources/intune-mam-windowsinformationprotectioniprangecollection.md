---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 722e96e69027cccb666bc789fc7516b914b975bb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752305"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="41e89-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="41e89-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="41e89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41e89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41e89-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41e89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41e89-106">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="41e89-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="41e89-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41e89-107">Properties</span></span>
|<span data-ttu-id="41e89-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41e89-108">Property</span></span>|<span data-ttu-id="41e89-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="41e89-109">Type</span></span>|<span data-ttu-id="41e89-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="41e89-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e89-111">displayName</span><span class="sxs-lookup"><span data-stu-id="41e89-111">displayName</span></span>|<span data-ttu-id="41e89-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41e89-112">String</span></span>|<span data-ttu-id="41e89-113">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="41e89-113">Display name</span></span>|
|<span data-ttu-id="41e89-114">ranges</span><span class="sxs-lookup"><span data-stu-id="41e89-114">ranges</span></span>|<span data-ttu-id="41e89-115">Coleção [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="41e89-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="41e89-116">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="41e89-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="41e89-117">Relações</span><span class="sxs-lookup"><span data-stu-id="41e89-117">Relationships</span></span>
<span data-ttu-id="41e89-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="41e89-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41e89-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41e89-119">JSON Representation</span></span>
<span data-ttu-id="41e89-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41e89-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.ipRange"
    }
  ]
}
```




