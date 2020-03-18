---
title: tipo de recurso edgeHomeButtonOpensCustomURL
description: Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ba83e4ee870a5e258a40c0c94d8d157f8564a91
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791888"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="97d43-103">tipo de recurso edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="97d43-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="97d43-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="97d43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97d43-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="97d43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97d43-106">Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.</span><span class="sxs-lookup"><span data-stu-id="97d43-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="97d43-107">Herda de [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97d43-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97d43-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97d43-108">Properties</span></span>
|<span data-ttu-id="97d43-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97d43-109">Property</span></span>|<span data-ttu-id="97d43-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="97d43-110">Type</span></span>|<span data-ttu-id="97d43-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="97d43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97d43-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="97d43-112">homeButtonCustomURL</span></span>|<span data-ttu-id="97d43-113">String</span><span class="sxs-lookup"><span data-stu-id="97d43-113">String</span></span>|<span data-ttu-id="97d43-114">A URL específica a ser carregada.</span><span class="sxs-lookup"><span data-stu-id="97d43-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97d43-115">Relações</span><span class="sxs-lookup"><span data-stu-id="97d43-115">Relationships</span></span>
<span data-ttu-id="97d43-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97d43-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97d43-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97d43-117">JSON Representation</span></span>
<span data-ttu-id="97d43-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97d43-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```



