---
title: tipo de recurso iosBookmark
description: indicador de URL iOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d0477665b0de7390cfe9d2f4453401d5db7d4946
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273701"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="7e9d7-103">tipo de recurso iosBookmark</span><span class="sxs-lookup"><span data-stu-id="7e9d7-103">iosBookmark resource type</span></span>

<span data-ttu-id="7e9d7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e9d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e9d7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7e9d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e9d7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e9d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e9d7-107">indicador de URL iOS</span><span class="sxs-lookup"><span data-stu-id="7e9d7-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="7e9d7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e9d7-108">Properties</span></span>
|<span data-ttu-id="7e9d7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e9d7-109">Property</span></span>|<span data-ttu-id="7e9d7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e9d7-110">Type</span></span>|<span data-ttu-id="7e9d7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e9d7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e9d7-112">url</span><span class="sxs-lookup"><span data-stu-id="7e9d7-112">url</span></span>|<span data-ttu-id="7e9d7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7e9d7-113">String</span></span>|<span data-ttu-id="7e9d7-114">URL com permissão para acessar</span><span class="sxs-lookup"><span data-stu-id="7e9d7-114">URL allowed to access</span></span>|
|<span data-ttu-id="7e9d7-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="7e9d7-115">bookmarkFolder</span></span>|<span data-ttu-id="7e9d7-116">String</span><span class="sxs-lookup"><span data-stu-id="7e9d7-116">String</span></span>|<span data-ttu-id="7e9d7-117">A pasta na qual o indicador deve ser adicionado no Safari</span><span class="sxs-lookup"><span data-stu-id="7e9d7-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="7e9d7-118">displayName</span><span class="sxs-lookup"><span data-stu-id="7e9d7-118">displayName</span></span>|<span data-ttu-id="7e9d7-119">String</span><span class="sxs-lookup"><span data-stu-id="7e9d7-119">String</span></span>|<span data-ttu-id="7e9d7-120">O nome de exibição do indicador</span><span class="sxs-lookup"><span data-stu-id="7e9d7-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e9d7-121">Relações</span><span class="sxs-lookup"><span data-stu-id="7e9d7-121">Relationships</span></span>
<span data-ttu-id="7e9d7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e9d7-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e9d7-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e9d7-123">JSON Representation</span></span>
<span data-ttu-id="7e9d7-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e9d7-124">Here is a JSON representation of the resource.</span></span>
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




