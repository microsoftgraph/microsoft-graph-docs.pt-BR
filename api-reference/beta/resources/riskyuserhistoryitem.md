---
title: tipo de recurso riskyUserHistoryItem
description: Representa o histórico de riscos de usuários do Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f91f07e889a1808696a0bfb7180b51aa06355334
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016161"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="3b3b0-103">tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="3b3b0-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="3b3b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b3b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="3b3b0-105">Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b3b0-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="3b3b0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3b3b0-106">Methods</span></span>

| <span data-ttu-id="3b3b0-107">Método</span><span class="sxs-lookup"><span data-stu-id="3b3b0-107">Method</span></span>   | <span data-ttu-id="3b3b0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3b3b0-108">Return Type</span></span>|<span data-ttu-id="3b3b0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b3b0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b3b0-110">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="3b3b0-110">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="3b3b0-111">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3b3b0-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="3b3b0-112">Obter o histórico de riscos de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3b3b0-112">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="3b3b0-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b3b0-113">Properties</span></span>

| <span data-ttu-id="3b3b0-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b3b0-114">Property</span></span>       | <span data-ttu-id="3b3b0-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b3b0-115">Type</span></span>    | <span data-ttu-id="3b3b0-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b3b0-116">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="3b3b0-117">userId</span><span class="sxs-lookup"><span data-stu-id="3b3b0-117">userId</span></span>         | <span data-ttu-id="3b3b0-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b3b0-118">string</span></span>  | <span data-ttu-id="3b3b0-119">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="3b3b0-119">The id of the user.</span></span> |
| <span data-ttu-id="3b3b0-120">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="3b3b0-120">initiatedBy</span></span>    | <span data-ttu-id="3b3b0-121">bool</span><span class="sxs-lookup"><span data-stu-id="3b3b0-121">bool</span></span>    | <span data-ttu-id="3b3b0-122">A ID do ator que faz a operação.</span><span class="sxs-lookup"><span data-stu-id="3b3b0-122">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="3b3b0-123">atividade</span><span class="sxs-lookup"><span data-stu-id="3b3b0-123">activity</span></span>       | [<span data-ttu-id="3b3b0-124">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="3b3b0-124">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="3b3b0-125">A atividade relacionada à alteração no nível de risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="3b3b0-125">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="3b3b0-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b3b0-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "string",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "riskyUserHistoryItem resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->


