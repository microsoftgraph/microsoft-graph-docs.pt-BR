---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c595256953928138ec140b799410f5ba43d0b3de
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950967"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="a13f1-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="a13f1-103">omaSetting resource type</span></span>

> <span data-ttu-id="a13f1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a13f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a13f1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a13f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a13f1-106">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="a13f1-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a13f1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a13f1-107">Properties</span></span>
|<span data-ttu-id="a13f1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a13f1-108">Property</span></span>|<span data-ttu-id="a13f1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a13f1-109">Type</span></span>|<span data-ttu-id="a13f1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a13f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a13f1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a13f1-111">displayName</span></span>|<span data-ttu-id="a13f1-112">String</span><span class="sxs-lookup"><span data-stu-id="a13f1-112">String</span></span>|<span data-ttu-id="a13f1-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a13f1-113">Display Name.</span></span>|
|<span data-ttu-id="a13f1-114">description</span><span class="sxs-lookup"><span data-stu-id="a13f1-114">description</span></span>|<span data-ttu-id="a13f1-115">String</span><span class="sxs-lookup"><span data-stu-id="a13f1-115">String</span></span>|<span data-ttu-id="a13f1-116">Descrição.</span><span class="sxs-lookup"><span data-stu-id="a13f1-116">Description.</span></span>|
|<span data-ttu-id="a13f1-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="a13f1-117">omaUri</span></span>|<span data-ttu-id="a13f1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a13f1-118">String</span></span>|<span data-ttu-id="a13f1-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="a13f1-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a13f1-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a13f1-120">Relationships</span></span>
<span data-ttu-id="a13f1-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a13f1-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a13f1-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a13f1-122">JSON Representation</span></span>
<span data-ttu-id="a13f1-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a13f1-123">Here is a JSON representation of the resource.</span></span>
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




