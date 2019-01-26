---
title: " tipo de recurso de secureScoreControlStateUpdate"
description: Este recurso contém o histórico de estados de controle atualizado por usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574387"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="c6a33-103">tipo de recurso de secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="c6a33-103">secureScoreControlStateUpdate resource type</span></span>

> <span data-ttu-id="c6a33-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c6a33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6a33-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c6a33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6a33-106">Contém o histórico dos Estados controle atualizados pelo usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).</span><span class="sxs-lookup"><span data-stu-id="c6a33-106">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="c6a33-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6a33-107">Property</span></span>         | <span data-ttu-id="c6a33-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6a33-108">Type</span></span>           |<span data-ttu-id="c6a33-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6a33-109">Description</span></span>                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| <span data-ttu-id="c6a33-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="c6a33-110">assignedTo</span></span>      | <span data-ttu-id="c6a33-111">string</span><span class="sxs-lookup"><span data-stu-id="c6a33-111">string</span></span>         | <span data-ttu-id="c6a33-112">Atribua o controle ao usuário que executará a ação</span><span class="sxs-lookup"><span data-stu-id="c6a33-112">Assign the control to the user who will take the action</span></span>     |
| <span data-ttu-id="c6a33-113">comment</span><span class="sxs-lookup"><span data-stu-id="c6a33-113">comment</span></span>         | <span data-ttu-id="c6a33-114">string</span><span class="sxs-lookup"><span data-stu-id="c6a33-114">string</span></span>         | <span data-ttu-id="c6a33-115">Fornece um comentário opcional sobre o controle</span><span class="sxs-lookup"><span data-stu-id="c6a33-115">Provides optional comment about the control</span></span>                 |
| <span data-ttu-id="c6a33-116">estado</span><span class="sxs-lookup"><span data-stu-id="c6a33-116">state</span></span>           | <span data-ttu-id="c6a33-117">string</span><span class="sxs-lookup"><span data-stu-id="c6a33-117">string</span></span>         | <span data-ttu-id="c6a33-118">Estado do controle pode ser modificado usando-se o comando de PATCH (ex.: ignorados, thirdParty etc.)</span><span class="sxs-lookup"><span data-stu-id="c6a33-118">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
| <span data-ttu-id="c6a33-119">updatedBy</span><span class="sxs-lookup"><span data-stu-id="c6a33-119">updatedBy</span></span>       | <span data-ttu-id="c6a33-120">string</span><span class="sxs-lookup"><span data-stu-id="c6a33-120">string</span></span>         |<span data-ttu-id="c6a33-121">ID do usuário que atualizou o estado de locatário</span><span class="sxs-lookup"><span data-stu-id="c6a33-121">ID of the user who updated tenant state</span></span>                      |
| <span data-ttu-id="c6a33-122">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6a33-122">updatedDateTime</span></span> | <span data-ttu-id="c6a33-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6a33-123">DateTimeOffset</span></span> |<span data-ttu-id="c6a33-124">Tempo no qual controle estado foi atualizado</span><span class="sxs-lookup"><span data-stu-id="c6a33-124">Time at which control state was updated</span></span>                      |
 

## <a name="json-representation"></a><span data-ttu-id="c6a33-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6a33-125">JSON representation</span></span>
 <span data-ttu-id="c6a33-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6a33-126">The following is a JSON representation of the resource.</span></span>

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "DateTimeOffset"
}
```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
