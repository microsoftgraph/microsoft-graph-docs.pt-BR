---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 411e3909a71d94be2c6086e9a00616245fca062b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525982"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="4415e-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="4415e-103">omaSetting resource type</span></span>

<span data-ttu-id="4415e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4415e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4415e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4415e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4415e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4415e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4415e-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="4415e-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="4415e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4415e-108">Properties</span></span>
|<span data-ttu-id="4415e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4415e-109">Property</span></span>|<span data-ttu-id="4415e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4415e-110">Type</span></span>|<span data-ttu-id="4415e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4415e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4415e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4415e-112">displayName</span></span>|<span data-ttu-id="4415e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4415e-113">String</span></span>|<span data-ttu-id="4415e-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="4415e-114">Display Name.</span></span>|
|<span data-ttu-id="4415e-115">description</span><span class="sxs-lookup"><span data-stu-id="4415e-115">description</span></span>|<span data-ttu-id="4415e-116">String</span><span class="sxs-lookup"><span data-stu-id="4415e-116">String</span></span>|<span data-ttu-id="4415e-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="4415e-117">Description.</span></span>|
|<span data-ttu-id="4415e-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="4415e-118">omaUri</span></span>|<span data-ttu-id="4415e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4415e-119">String</span></span>|<span data-ttu-id="4415e-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="4415e-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4415e-121">Relações</span><span class="sxs-lookup"><span data-stu-id="4415e-121">Relationships</span></span>
<span data-ttu-id="4415e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4415e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4415e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4415e-123">JSON Representation</span></span>
<span data-ttu-id="4415e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4415e-124">Here is a JSON representation of the resource.</span></span>
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



