---
title: " tipo de recurso de controlScore"
description: Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034472"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="83de0-103">tipo de recurso de controlScore</span><span class="sxs-lookup"><span data-stu-id="83de0-103">controlScore resource type</span></span>

<span data-ttu-id="83de0-104">Este recurso contém uma pontuação de locatário e uma descrição para um controle individual.</span><span class="sxs-lookup"><span data-stu-id="83de0-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="83de0-105">Nome</span><span class="sxs-lookup"><span data-stu-id="83de0-105">Name</span></span> |<span data-ttu-id="83de0-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="83de0-106">Type</span></span> |<span data-ttu-id="83de0-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="83de0-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="83de0-108">controlName</span><span class="sxs-lookup"><span data-stu-id="83de0-108">controlName</span></span> |   <span data-ttu-id="83de0-109">String</span><span class="sxs-lookup"><span data-stu-id="83de0-109">String</span></span>  |   <span data-ttu-id="83de0-110">Nome exclusivo do controle</span><span class="sxs-lookup"><span data-stu-id="83de0-110">Control unique name</span></span> |
|   <span data-ttu-id="83de0-111">score</span><span class="sxs-lookup"><span data-stu-id="83de0-111">score</span></span>   |   <span data-ttu-id="83de0-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="83de0-112">Double</span></span>  |  <span data-ttu-id="83de0-113">Locatário alcançado e pontuação para o controle (ele diariamente varia dependendo de operações de Inquilino no controle).</span><span class="sxs-lookup"><span data-stu-id="83de0-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="83de0-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="83de0-114">controlCategory</span></span> |   <span data-ttu-id="83de0-115">String</span><span class="sxs-lookup"><span data-stu-id="83de0-115">String</span></span>  |  <span data-ttu-id="83de0-116">Categoria de ação de controle (identidade, dados, dispositivo, aplicativos, infra-estrutura).</span><span class="sxs-lookup"><span data-stu-id="83de0-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="83de0-117">description</span><span class="sxs-lookup"><span data-stu-id="83de0-117">description</span></span> |   <span data-ttu-id="83de0-118">String</span><span class="sxs-lookup"><span data-stu-id="83de0-118">String</span></span>  |  <span data-ttu-id="83de0-119">Descrição do controle.</span><span class="sxs-lookup"><span data-stu-id="83de0-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83de0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83de0-120">JSON representation</span></span>

<span data-ttu-id="83de0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83de0-121">The following is a JSON representation of the resource.</span></span>

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
