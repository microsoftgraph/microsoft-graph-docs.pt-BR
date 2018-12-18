---
title: insightIdentity
description: Tipo complexo que contém as propriedades de itens compartilhados.
author: simonhult
ms.openlocfilehash: 648242b827c0390029522955b0fe6347b98100c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331329"
---
# <a name="insightidentity"></a><span data-ttu-id="6428e-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="6428e-103">insightIdentity</span></span>

> <span data-ttu-id="6428e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6428e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6428e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6428e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6428e-106">Tipo complexo que contém as propriedades de itens [compartilhados](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="6428e-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="6428e-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6428e-107">JSON representation</span></span>
<span data-ttu-id="6428e-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6428e-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6428e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6428e-109">Properties</span></span>

| <span data-ttu-id="6428e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6428e-110">Property</span></span>              | <span data-ttu-id="6428e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6428e-111">Type</span></span>          | <span data-ttu-id="6428e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6428e-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="6428e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6428e-113">displayName</span></span>       | <span data-ttu-id="6428e-114">String</span><span class="sxs-lookup"><span data-stu-id="6428e-114">String</span></span>          | <span data-ttu-id="6428e-115">O nome de exibição do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="6428e-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="6428e-116">id</span><span class="sxs-lookup"><span data-stu-id="6428e-116">id</span></span>              | <span data-ttu-id="6428e-117">String</span><span class="sxs-lookup"><span data-stu-id="6428e-117">String</span></span>        | <span data-ttu-id="6428e-118">A identificação do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="6428e-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="6428e-119">address</span><span class="sxs-lookup"><span data-stu-id="6428e-119">address</span></span>             | <span data-ttu-id="6428e-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6428e-120">String</span></span>      | <span data-ttu-id="6428e-121">O endereço de email do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="6428e-121">The email address of the user who shared the item.</span></span>  |