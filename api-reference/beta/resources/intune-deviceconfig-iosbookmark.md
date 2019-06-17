---
title: tipo de recurso iosBookmark
description: indicador de URL iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2f96b872d09eaf3c954f18a31219d6bfe17ddb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988360"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="da9f5-103">tipo de recurso iosBookmark</span><span class="sxs-lookup"><span data-stu-id="da9f5-103">iosBookmark resource type</span></span>

> <span data-ttu-id="da9f5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da9f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da9f5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da9f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da9f5-106">indicador de URL iOS</span><span class="sxs-lookup"><span data-stu-id="da9f5-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="da9f5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da9f5-107">Properties</span></span>
|<span data-ttu-id="da9f5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da9f5-108">Property</span></span>|<span data-ttu-id="da9f5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="da9f5-109">Type</span></span>|<span data-ttu-id="da9f5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="da9f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da9f5-111">url</span><span class="sxs-lookup"><span data-stu-id="da9f5-111">url</span></span>|<span data-ttu-id="da9f5-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da9f5-112">String</span></span>|<span data-ttu-id="da9f5-113">URL com permissão para acessar</span><span class="sxs-lookup"><span data-stu-id="da9f5-113">URL allowed to access</span></span>|
|<span data-ttu-id="da9f5-114">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="da9f5-114">bookmarkFolder</span></span>|<span data-ttu-id="da9f5-115">String</span><span class="sxs-lookup"><span data-stu-id="da9f5-115">String</span></span>|<span data-ttu-id="da9f5-116">A pasta na qual o indicador deve ser adicionado no Safari</span><span class="sxs-lookup"><span data-stu-id="da9f5-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="da9f5-117">displayName</span><span class="sxs-lookup"><span data-stu-id="da9f5-117">displayName</span></span>|<span data-ttu-id="da9f5-118">String</span><span class="sxs-lookup"><span data-stu-id="da9f5-118">String</span></span>|<span data-ttu-id="da9f5-119">O nome de exibição do indicador</span><span class="sxs-lookup"><span data-stu-id="da9f5-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="da9f5-120">Relações</span><span class="sxs-lookup"><span data-stu-id="da9f5-120">Relationships</span></span>
<span data-ttu-id="da9f5-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da9f5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da9f5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da9f5-122">JSON Representation</span></span>
<span data-ttu-id="da9f5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da9f5-123">Here is a JSON representation of the resource.</span></span>
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





