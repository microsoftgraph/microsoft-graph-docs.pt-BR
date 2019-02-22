---
title: tipo de recurso edgeHomeButtonOpensCustomURL
description: Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83fd3dbb0961011584ef9d65e01c361ccf6a228
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143236"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="2d9b7-103">tipo de recurso edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="2d9b7-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="2d9b7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d9b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d9b7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d9b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d9b7-106">Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.</span><span class="sxs-lookup"><span data-stu-id="2d9b7-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="2d9b7-107">Herda de [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d9b7-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2d9b7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d9b7-108">Properties</span></span>
|<span data-ttu-id="2d9b7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d9b7-109">Property</span></span>|<span data-ttu-id="2d9b7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d9b7-110">Type</span></span>|<span data-ttu-id="2d9b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d9b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d9b7-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="2d9b7-112">homeButtonCustomURL</span></span>|<span data-ttu-id="2d9b7-113">String</span><span class="sxs-lookup"><span data-stu-id="2d9b7-113">String</span></span>|<span data-ttu-id="2d9b7-114">A URL específica a ser carregada.</span><span class="sxs-lookup"><span data-stu-id="2d9b7-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d9b7-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2d9b7-115">Relationships</span></span>
<span data-ttu-id="2d9b7-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d9b7-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d9b7-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d9b7-117">JSON Representation</span></span>
<span data-ttu-id="2d9b7-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d9b7-118">Here is a JSON representation of the resource.</span></span>
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




