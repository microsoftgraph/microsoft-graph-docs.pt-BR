---
title: Tipo de recurso publicError
description: Representa um erro genérico e seus detalhes.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: e9f5decf8edc2ebf3e11d00eb89e68236a6a73d4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467237"
---
# <a name="publicerror-resource-type"></a><span data-ttu-id="9aab9-103">Tipo de recurso publicError</span><span class="sxs-lookup"><span data-stu-id="9aab9-103">publicError resource type</span></span>

<span data-ttu-id="9aab9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9aab9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9aab9-105">Representa um erro genérico e seus detalhes.</span><span class="sxs-lookup"><span data-stu-id="9aab9-105">Represents a generic error and its details.</span></span>

## <a name="properties"></a><span data-ttu-id="9aab9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9aab9-106">Properties</span></span>
|<span data-ttu-id="9aab9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9aab9-107">Property</span></span>|<span data-ttu-id="9aab9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aab9-108">Type</span></span>|<span data-ttu-id="9aab9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aab9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aab9-110">código</span><span class="sxs-lookup"><span data-stu-id="9aab9-110">code</span></span>|<span data-ttu-id="9aab9-111">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aab9-111">string</span></span>| <span data-ttu-id="9aab9-112">Representa o código de erro.</span><span class="sxs-lookup"><span data-stu-id="9aab9-112">Represents the error code.</span></span>
|<span data-ttu-id="9aab9-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="9aab9-113">details</span></span>|<span data-ttu-id="9aab9-114">[Coleção publicErrorDetail](publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="9aab9-114">[publicErrorDetail](publicerrordetail.md) collection</span></span>|<span data-ttu-id="9aab9-115">Detalhes do erro.</span><span class="sxs-lookup"><span data-stu-id="9aab9-115">Details of the error.</span></span>|
|<span data-ttu-id="9aab9-116">innerError</span><span class="sxs-lookup"><span data-stu-id="9aab9-116">innerError</span></span>|[<span data-ttu-id="9aab9-117">publicInnerError</span><span class="sxs-lookup"><span data-stu-id="9aab9-117">publicInnerError</span></span>](publicinnererror.md)|<span data-ttu-id="9aab9-118">Detalhes do erro interno.</span><span class="sxs-lookup"><span data-stu-id="9aab9-118">Details of the inner error.</span></span>|
|<span data-ttu-id="9aab9-119">mensagem</span><span class="sxs-lookup"><span data-stu-id="9aab9-119">message</span></span>|<span data-ttu-id="9aab9-120">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aab9-120">string</span></span>| <span data-ttu-id="9aab9-121">Uma mensagem não localizada para o desenvolvedor.</span><span class="sxs-lookup"><span data-stu-id="9aab9-121">A non-localized message for the developer.</span></span>
|<span data-ttu-id="9aab9-122">destino</span><span class="sxs-lookup"><span data-stu-id="9aab9-122">target</span></span>|<span data-ttu-id="9aab9-123">String</span><span class="sxs-lookup"><span data-stu-id="9aab9-123">String</span></span>|<span data-ttu-id="9aab9-124">O destino do erro.</span><span class="sxs-lookup"><span data-stu-id="9aab9-124">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aab9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="9aab9-125">Relationships</span></span>
<span data-ttu-id="9aab9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9aab9-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9aab9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9aab9-127">JSON representation</span></span>
<span data-ttu-id="9aab9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9aab9-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ],
  "innerError": {
    "@odata.type": "microsoft.graph.publicInnerError"
  }
}
```
