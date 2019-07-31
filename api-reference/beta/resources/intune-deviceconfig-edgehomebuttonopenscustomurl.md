---
title: tipo de recurso edgeHomeButtonOpensCustomURL
description: Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88310056a70231c0f536420b87fbecff05b73b42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001450"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="53e3a-103">tipo de recurso edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="53e3a-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="53e3a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53e3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53e3a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53e3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e3a-106">Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.</span><span class="sxs-lookup"><span data-stu-id="53e3a-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="53e3a-107">Herda de [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53e3a-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="53e3a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53e3a-108">Properties</span></span>
|<span data-ttu-id="53e3a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53e3a-109">Property</span></span>|<span data-ttu-id="53e3a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="53e3a-110">Type</span></span>|<span data-ttu-id="53e3a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="53e3a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e3a-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="53e3a-112">homeButtonCustomURL</span></span>|<span data-ttu-id="53e3a-113">String</span><span class="sxs-lookup"><span data-stu-id="53e3a-113">String</span></span>|<span data-ttu-id="53e3a-114">A URL específica a ser carregada.</span><span class="sxs-lookup"><span data-stu-id="53e3a-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53e3a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="53e3a-115">Relationships</span></span>
<span data-ttu-id="53e3a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53e3a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53e3a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53e3a-117">JSON Representation</span></span>
<span data-ttu-id="53e3a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53e3a-118">Here is a JSON representation of the resource.</span></span>
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





