---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 34137caf93bcdd3a3621842b9976e964b8f44c78
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759991"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="a2f27-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="a2f27-103">omaSetting resource type</span></span>

<span data-ttu-id="a2f27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2f27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2f27-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2f27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2f27-106">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="a2f27-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a2f27-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2f27-107">Properties</span></span>
|<span data-ttu-id="a2f27-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2f27-108">Property</span></span>|<span data-ttu-id="a2f27-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2f27-109">Type</span></span>|<span data-ttu-id="a2f27-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2f27-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2f27-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a2f27-111">displayName</span></span>|<span data-ttu-id="a2f27-112">String</span><span class="sxs-lookup"><span data-stu-id="a2f27-112">String</span></span>|<span data-ttu-id="a2f27-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="a2f27-113">Display Name.</span></span>|
|<span data-ttu-id="a2f27-114">description</span><span class="sxs-lookup"><span data-stu-id="a2f27-114">description</span></span>|<span data-ttu-id="a2f27-115">String</span><span class="sxs-lookup"><span data-stu-id="a2f27-115">String</span></span>|<span data-ttu-id="a2f27-116">Descrição.</span><span class="sxs-lookup"><span data-stu-id="a2f27-116">Description.</span></span>|
|<span data-ttu-id="a2f27-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="a2f27-117">omaUri</span></span>|<span data-ttu-id="a2f27-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2f27-118">String</span></span>|<span data-ttu-id="a2f27-119">OMA.</span><span class="sxs-lookup"><span data-stu-id="a2f27-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2f27-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a2f27-120">Relationships</span></span>
<span data-ttu-id="a2f27-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2f27-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2f27-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2f27-122">JSON Representation</span></span>
<span data-ttu-id="a2f27-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2f27-123">Here is a JSON representation of the resource.</span></span>
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




