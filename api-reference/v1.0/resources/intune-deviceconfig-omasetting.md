---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e49aa085eb0cf23384bbed739235df46e5da1f72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978171"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="f52f8-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="f52f8-103">omaSetting resource type</span></span>

<span data-ttu-id="f52f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f52f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f52f8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f52f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f52f8-106">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="f52f8-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="f52f8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f52f8-107">Properties</span></span>
|<span data-ttu-id="f52f8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f52f8-108">Property</span></span>|<span data-ttu-id="f52f8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f52f8-109">Type</span></span>|<span data-ttu-id="f52f8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f52f8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f52f8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f52f8-111">displayName</span></span>|<span data-ttu-id="f52f8-112">String</span><span class="sxs-lookup"><span data-stu-id="f52f8-112">String</span></span>|<span data-ttu-id="f52f8-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f52f8-113">Display Name.</span></span>|
|<span data-ttu-id="f52f8-114">description</span><span class="sxs-lookup"><span data-stu-id="f52f8-114">description</span></span>|<span data-ttu-id="f52f8-115">String</span><span class="sxs-lookup"><span data-stu-id="f52f8-115">String</span></span>|<span data-ttu-id="f52f8-116">Descrição.</span><span class="sxs-lookup"><span data-stu-id="f52f8-116">Description.</span></span>|
|<span data-ttu-id="f52f8-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="f52f8-117">omaUri</span></span>|<span data-ttu-id="f52f8-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f52f8-118">String</span></span>|<span data-ttu-id="f52f8-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="f52f8-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f52f8-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f52f8-120">Relationships</span></span>
<span data-ttu-id="f52f8-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f52f8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f52f8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f52f8-122">JSON Representation</span></span>
<span data-ttu-id="f52f8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f52f8-123">Here is a JSON representation of the resource.</span></span>
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









