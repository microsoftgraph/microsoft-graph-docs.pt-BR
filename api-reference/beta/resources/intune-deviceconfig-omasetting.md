---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fab80ad06fb5654578f29b92e3b0f3aa9c09abdb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143845"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="fff34-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="fff34-103">omaSetting resource type</span></span>

> <span data-ttu-id="fff34-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fff34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fff34-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fff34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fff34-106">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="fff34-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="fff34-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fff34-107">Properties</span></span>
|<span data-ttu-id="fff34-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fff34-108">Property</span></span>|<span data-ttu-id="fff34-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fff34-109">Type</span></span>|<span data-ttu-id="fff34-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fff34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fff34-111">displayName</span><span class="sxs-lookup"><span data-stu-id="fff34-111">displayName</span></span>|<span data-ttu-id="fff34-112">String</span><span class="sxs-lookup"><span data-stu-id="fff34-112">String</span></span>|<span data-ttu-id="fff34-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="fff34-113">Display Name.</span></span>|
|<span data-ttu-id="fff34-114">descrição</span><span class="sxs-lookup"><span data-stu-id="fff34-114">description</span></span>|<span data-ttu-id="fff34-115">String</span><span class="sxs-lookup"><span data-stu-id="fff34-115">String</span></span>|<span data-ttu-id="fff34-116">Descrição.</span><span class="sxs-lookup"><span data-stu-id="fff34-116">Description.</span></span>|
|<span data-ttu-id="fff34-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="fff34-117">omaUri</span></span>|<span data-ttu-id="fff34-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fff34-118">String</span></span>|<span data-ttu-id="fff34-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="fff34-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fff34-120">Relações</span><span class="sxs-lookup"><span data-stu-id="fff34-120">Relationships</span></span>
<span data-ttu-id="fff34-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fff34-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fff34-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fff34-122">JSON Representation</span></span>
<span data-ttu-id="fff34-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fff34-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```




