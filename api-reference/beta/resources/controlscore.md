---
title: " tipo de recurso de controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891466"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="6723d-103">tipo de recurso de controlScore</span><span class="sxs-lookup"><span data-stu-id="6723d-103">controlScore resource type</span></span>

<span data-ttu-id="6723d-104">Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="6723d-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="6723d-105">Nome</span><span class="sxs-lookup"><span data-stu-id="6723d-105">Name</span></span> |<span data-ttu-id="6723d-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="6723d-106">Type</span></span> |<span data-ttu-id="6723d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="6723d-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6723d-108">controlName</span><span class="sxs-lookup"><span data-stu-id="6723d-108">controlName</span></span> |   <span data-ttu-id="6723d-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6723d-109">String</span></span>  |   <span data-ttu-id="6723d-110">Nome exclusivo do controle</span><span class="sxs-lookup"><span data-stu-id="6723d-110">Control unique name</span></span> |
|   <span data-ttu-id="6723d-111">score</span><span class="sxs-lookup"><span data-stu-id="6723d-111">score</span></span>   |   <span data-ttu-id="6723d-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="6723d-112">Double</span></span>  |  <span data-ttu-id="6723d-113">Locatário alcançado e pontuação para o controle (ele diariamente varia dependendo de operações de Inquilino no controle).</span><span class="sxs-lookup"><span data-stu-id="6723d-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="6723d-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="6723d-114">controlCategory</span></span> |   <span data-ttu-id="6723d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6723d-115">String</span></span>  |  <span data-ttu-id="6723d-116">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura).</span><span class="sxs-lookup"><span data-stu-id="6723d-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="6723d-117">description</span><span class="sxs-lookup"><span data-stu-id="6723d-117">description</span></span> |   <span data-ttu-id="6723d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6723d-118">String</span></span>  |  <span data-ttu-id="6723d-119">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="6723d-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6723d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6723d-120">JSON representation</span></span>

<span data-ttu-id="6723d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6723d-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "String",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
