---
title: tipo de recurso iosBookmark
description: indicador de URL iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7bfc889acd17049e38a0e4efe03d83389e9983fd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729673"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="e7076-103">tipo de recurso iosBookmark</span><span class="sxs-lookup"><span data-stu-id="e7076-103">iosBookmark resource type</span></span>

<span data-ttu-id="e7076-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7076-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7076-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7076-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7076-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7076-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7076-107">indicador de URL iOS</span><span class="sxs-lookup"><span data-stu-id="e7076-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="e7076-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7076-108">Properties</span></span>
|<span data-ttu-id="e7076-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7076-109">Property</span></span>|<span data-ttu-id="e7076-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7076-110">Type</span></span>|<span data-ttu-id="e7076-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7076-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7076-112">url</span><span class="sxs-lookup"><span data-stu-id="e7076-112">url</span></span>|<span data-ttu-id="e7076-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e7076-113">String</span></span>|<span data-ttu-id="e7076-114">URL com permissão para acessar</span><span class="sxs-lookup"><span data-stu-id="e7076-114">URL allowed to access</span></span>|
|<span data-ttu-id="e7076-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="e7076-115">bookmarkFolder</span></span>|<span data-ttu-id="e7076-116">String</span><span class="sxs-lookup"><span data-stu-id="e7076-116">String</span></span>|<span data-ttu-id="e7076-117">A pasta na qual o indicador deve ser adicionado no Safari</span><span class="sxs-lookup"><span data-stu-id="e7076-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="e7076-118">displayName</span><span class="sxs-lookup"><span data-stu-id="e7076-118">displayName</span></span>|<span data-ttu-id="e7076-119">String</span><span class="sxs-lookup"><span data-stu-id="e7076-119">String</span></span>|<span data-ttu-id="e7076-120">O nome de exibição do indicador</span><span class="sxs-lookup"><span data-stu-id="e7076-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7076-121">Relações</span><span class="sxs-lookup"><span data-stu-id="e7076-121">Relationships</span></span>
<span data-ttu-id="e7076-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7076-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7076-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7076-123">JSON Representation</span></span>
<span data-ttu-id="e7076-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7076-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```





