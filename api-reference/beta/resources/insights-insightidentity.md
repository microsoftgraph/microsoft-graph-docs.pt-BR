---
title: insightIdentity
description: " tipo de recurso"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037747"
---
# <a name="insightidentity"></a><span data-ttu-id="227a4-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="227a4-103">insightIdentity</span></span>

> <span data-ttu-id="227a4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="227a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="227a4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="227a4-105">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="227a4-106">tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="227a4-106">resource type</span></span>

<span data-ttu-id="227a4-107">Tipo complexo que contém as propriedades de itens [compartilhados](insights-shared.md) .</span><span class="sxs-lookup"><span data-stu-id="227a4-107">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="227a4-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="227a4-108">JSON representation</span></span>
<span data-ttu-id="227a4-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="227a4-109">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="227a4-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="227a4-110">Properties</span></span>

| <span data-ttu-id="227a4-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="227a4-111">Property</span></span>              | <span data-ttu-id="227a4-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="227a4-112">Type</span></span>          | <span data-ttu-id="227a4-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="227a4-113">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="227a4-114">displayName</span><span class="sxs-lookup"><span data-stu-id="227a4-114">displayName</span></span>       | <span data-ttu-id="227a4-115">String</span><span class="sxs-lookup"><span data-stu-id="227a4-115">String</span></span>          | <span data-ttu-id="227a4-116">O nome de exibição do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="227a4-116">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="227a4-117">id</span><span class="sxs-lookup"><span data-stu-id="227a4-117">id</span></span>              | <span data-ttu-id="227a4-118">String</span><span class="sxs-lookup"><span data-stu-id="227a4-118">String</span></span>        | <span data-ttu-id="227a4-119">A identificação do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="227a4-119">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="227a4-120">address</span><span class="sxs-lookup"><span data-stu-id="227a4-120">address</span></span>             | <span data-ttu-id="227a4-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="227a4-121">String</span></span>      | <span data-ttu-id="227a4-122">O endereço de email do usuário que shared o item.</span><span class="sxs-lookup"><span data-stu-id="227a4-122">The email address of the user who shared the item.</span></span>  |