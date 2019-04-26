---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d0a69c10f1f0075caee48276bdbc37f6d616f22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549549"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="613c9-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="613c9-103">omaSetting resource type</span></span>

> <span data-ttu-id="613c9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="613c9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="613c9-105">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="613c9-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="613c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="613c9-106">Properties</span></span>
|<span data-ttu-id="613c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="613c9-107">Property</span></span>|<span data-ttu-id="613c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="613c9-108">Type</span></span>|<span data-ttu-id="613c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="613c9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="613c9-110">displayName</span><span class="sxs-lookup"><span data-stu-id="613c9-110">displayName</span></span>|<span data-ttu-id="613c9-111">String</span><span class="sxs-lookup"><span data-stu-id="613c9-111">String</span></span>|<span data-ttu-id="613c9-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="613c9-112">Display Name.</span></span>|
|<span data-ttu-id="613c9-113">description</span><span class="sxs-lookup"><span data-stu-id="613c9-113">description</span></span>|<span data-ttu-id="613c9-114">String</span><span class="sxs-lookup"><span data-stu-id="613c9-114">String</span></span>|<span data-ttu-id="613c9-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="613c9-115">Description.</span></span>|
|<span data-ttu-id="613c9-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="613c9-116">omaUri</span></span>|<span data-ttu-id="613c9-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="613c9-117">String</span></span>|<span data-ttu-id="613c9-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="613c9-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="613c9-119">Relações</span><span class="sxs-lookup"><span data-stu-id="613c9-119">Relationships</span></span>
<span data-ttu-id="613c9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="613c9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="613c9-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="613c9-121">JSON Representation</span></span>
<span data-ttu-id="613c9-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="613c9-122">Here is a JSON representation of the resource.</span></span>
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



