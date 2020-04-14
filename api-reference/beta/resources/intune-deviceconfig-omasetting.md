---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bfd4c72bc6018a4b49bcc20c0c1abd953052e471
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402033"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="65c1b-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="65c1b-103">omaSetting resource type</span></span>

<span data-ttu-id="65c1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65c1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65c1b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="65c1b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65c1b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65c1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65c1b-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="65c1b-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="65c1b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65c1b-108">Properties</span></span>
|<span data-ttu-id="65c1b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65c1b-109">Property</span></span>|<span data-ttu-id="65c1b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="65c1b-110">Type</span></span>|<span data-ttu-id="65c1b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65c1b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65c1b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="65c1b-112">displayName</span></span>|<span data-ttu-id="65c1b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65c1b-113">String</span></span>|<span data-ttu-id="65c1b-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="65c1b-114">Display Name.</span></span>|
|<span data-ttu-id="65c1b-115">description</span><span class="sxs-lookup"><span data-stu-id="65c1b-115">description</span></span>|<span data-ttu-id="65c1b-116">String</span><span class="sxs-lookup"><span data-stu-id="65c1b-116">String</span></span>|<span data-ttu-id="65c1b-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="65c1b-117">Description.</span></span>|
|<span data-ttu-id="65c1b-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="65c1b-118">omaUri</span></span>|<span data-ttu-id="65c1b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="65c1b-119">String</span></span>|<span data-ttu-id="65c1b-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="65c1b-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65c1b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="65c1b-121">Relationships</span></span>
<span data-ttu-id="65c1b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65c1b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65c1b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65c1b-123">JSON Representation</span></span>
<span data-ttu-id="65c1b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65c1b-124">Here is a JSON representation of the resource.</span></span>
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



