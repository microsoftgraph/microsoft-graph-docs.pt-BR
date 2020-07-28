---
title: tipo de recurso signInFrequencySessionControl
description: Controle de sessão para impor a frequência de entrada.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af2d23c26d2911c8abc36c8a9e66fb776edd43e0
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434845"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="12e81-103">tipo de recurso signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="12e81-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="12e81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12e81-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12e81-105">Controle de sessão para impor frequência de logon.</span><span class="sxs-lookup"><span data-stu-id="12e81-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="12e81-106">Herda do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="12e81-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="12e81-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12e81-107">Properties</span></span>

| <span data-ttu-id="12e81-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12e81-108">Property</span></span>     | <span data-ttu-id="12e81-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="12e81-109">Type</span></span>        | <span data-ttu-id="12e81-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e81-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12e81-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="12e81-111">isEnabled</span></span>     |<span data-ttu-id="12e81-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="12e81-112">Boolean</span></span>      | <span data-ttu-id="12e81-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="12e81-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="12e81-114">tipo</span><span class="sxs-lookup"><span data-stu-id="12e81-114">type</span></span>          |<span data-ttu-id="12e81-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12e81-115">String</span></span>       | <span data-ttu-id="12e81-116">Os valores possíveis são: `days` e `hours`.</span><span class="sxs-lookup"><span data-stu-id="12e81-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="12e81-117">valor</span><span class="sxs-lookup"><span data-stu-id="12e81-117">value</span></span>         |<span data-ttu-id="12e81-118">Int32</span><span class="sxs-lookup"><span data-stu-id="12e81-118">Int32</span></span>        | <span data-ttu-id="12e81-119">O número de `days` ou `hours` .</span><span class="sxs-lookup"><span data-stu-id="12e81-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12e81-120">Relações</span><span class="sxs-lookup"><span data-stu-id="12e81-120">Relationships</span></span>

<span data-ttu-id="12e81-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12e81-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12e81-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12e81-122">JSON representation</span></span>

<span data-ttu-id="12e81-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12e81-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "type": "String",
  "value": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
