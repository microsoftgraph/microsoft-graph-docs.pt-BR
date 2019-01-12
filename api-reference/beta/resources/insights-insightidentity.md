---
title: insightIdentity
description: Tipo complexo que contém as propriedades de itens compartilhados.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a263caa68280128a67a027b75682407fd4932605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938934"
---
# <a name="insightidentity"></a><span data-ttu-id="6a6ac-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="6a6ac-103">insightIdentity</span></span>

> <span data-ttu-id="6a6ac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a6ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a6ac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a6ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a6ac-106">Tipo complexo que contém as propriedades de itens [compartilhados](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="6a6ac-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="6a6ac-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a6ac-107">JSON representation</span></span>
<span data-ttu-id="6a6ac-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6a6ac-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6a6ac-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a6ac-109">Properties</span></span>

| <span data-ttu-id="6a6ac-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a6ac-110">Property</span></span>              | <span data-ttu-id="6a6ac-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a6ac-111">Type</span></span>          | <span data-ttu-id="6a6ac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a6ac-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="6a6ac-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6a6ac-113">displayName</span></span>       | <span data-ttu-id="6a6ac-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a6ac-114">String</span></span>          | <span data-ttu-id="6a6ac-115">O nome de exibição do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="6a6ac-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="6a6ac-116">id</span><span class="sxs-lookup"><span data-stu-id="6a6ac-116">id</span></span>              | <span data-ttu-id="6a6ac-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a6ac-117">String</span></span>        | <span data-ttu-id="6a6ac-118">A identificação do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="6a6ac-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="6a6ac-119">address</span><span class="sxs-lookup"><span data-stu-id="6a6ac-119">address</span></span>             | <span data-ttu-id="6a6ac-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a6ac-120">String</span></span>      | <span data-ttu-id="6a6ac-121">O endereço de email do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="6a6ac-121">The email address of the user who shared the item.</span></span>  |
