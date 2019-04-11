---
title: tipo de recurso edgeHomeButtonOpensCustomURL
description: Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dad4baba5fd55b99efd6b2b7ebadf1973d6c9c8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783712"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="e2d49-103">tipo de recurso edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="e2d49-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="e2d49-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2d49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2d49-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2d49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2d49-106">Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.</span><span class="sxs-lookup"><span data-stu-id="e2d49-106">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="e2d49-107">Herda de [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2d49-107">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2d49-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2d49-108">Properties</span></span>
|<span data-ttu-id="e2d49-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2d49-109">Property</span></span>|<span data-ttu-id="e2d49-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2d49-110">Type</span></span>|<span data-ttu-id="e2d49-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2d49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2d49-112">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="e2d49-112">homeButtonCustomURL</span></span>|<span data-ttu-id="e2d49-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2d49-113">String</span></span>|<span data-ttu-id="e2d49-114">A URL específica a ser carregada.</span><span class="sxs-lookup"><span data-stu-id="e2d49-114">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2d49-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e2d49-115">Relationships</span></span>
<span data-ttu-id="e2d49-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e2d49-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2d49-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2d49-117">JSON Representation</span></span>
<span data-ttu-id="e2d49-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2d49-118">Here is a JSON representation of the resource.</span></span>
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





