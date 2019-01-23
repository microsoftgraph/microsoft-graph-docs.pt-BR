---
title: tipo de recurso de edgeHomeButtonOpensCustomURL
description: Mostra o botão residencial; clicar no botão residencial carrega uma URL específica.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06f73375772f53b546e7e9b758a7513366949326
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431315"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="e1bb3-103">tipo de recurso de edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="e1bb3-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="e1bb3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1bb3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1bb3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1bb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1bb3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e1bb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1bb3-107">Mostra o botão residencial; clicar no botão residencial carrega uma URL específica.</span><span class="sxs-lookup"><span data-stu-id="e1bb3-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="e1bb3-108">Herda de [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e1bb3-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1bb3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1bb3-109">Properties</span></span>
|<span data-ttu-id="e1bb3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1bb3-110">Property</span></span>|<span data-ttu-id="e1bb3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1bb3-111">Type</span></span>|<span data-ttu-id="e1bb3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1bb3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1bb3-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="e1bb3-113">homeButtonCustomURL</span></span>|<span data-ttu-id="e1bb3-114">String</span><span class="sxs-lookup"><span data-stu-id="e1bb3-114">String</span></span>|<span data-ttu-id="e1bb3-115">A URL específica ao carregar.</span><span class="sxs-lookup"><span data-stu-id="e1bb3-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1bb3-116">Relações</span><span class="sxs-lookup"><span data-stu-id="e1bb3-116">Relationships</span></span>
<span data-ttu-id="e1bb3-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1bb3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1bb3-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1bb3-118">JSON Representation</span></span>
<span data-ttu-id="e1bb3-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1bb3-119">Here is a JSON representation of the resource.</span></span>
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




