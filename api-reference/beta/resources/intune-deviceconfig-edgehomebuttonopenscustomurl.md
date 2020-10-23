---
title: tipo de recurso edgeHomeButtonOpensCustomURL
description: Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f6bd4db13fad2863ffa6661fb9273085f70b7c0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732583"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="c0ed7-103">tipo de recurso edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="c0ed7-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="c0ed7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0ed7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0ed7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0ed7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0ed7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0ed7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0ed7-107">Mostrar o botão página inicial; clicar no botão página inicial carrega uma URL específica.</span><span class="sxs-lookup"><span data-stu-id="c0ed7-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="c0ed7-108">Herda de [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c0ed7-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0ed7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0ed7-109">Properties</span></span>
|<span data-ttu-id="c0ed7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0ed7-110">Property</span></span>|<span data-ttu-id="c0ed7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0ed7-111">Type</span></span>|<span data-ttu-id="c0ed7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0ed7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0ed7-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="c0ed7-113">homeButtonCustomURL</span></span>|<span data-ttu-id="c0ed7-114">String</span><span class="sxs-lookup"><span data-stu-id="c0ed7-114">String</span></span>|<span data-ttu-id="c0ed7-115">A URL específica a ser carregada.</span><span class="sxs-lookup"><span data-stu-id="c0ed7-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0ed7-116">Relações</span><span class="sxs-lookup"><span data-stu-id="c0ed7-116">Relationships</span></span>
<span data-ttu-id="c0ed7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0ed7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0ed7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0ed7-118">JSON Representation</span></span>
<span data-ttu-id="c0ed7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0ed7-119">Here is a JSON representation of the resource.</span></span>
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





