---
title: Tipo de recurso riskyUserHistoryItem
description: Representa o histórico de riscos dos usuários do Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4ae6d5fbc28e8dddb4c782aa9e9b2fad79b347ad
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442849"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="432d1-103">Tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="432d1-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="432d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="432d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="432d1-105">Representa o histórico de risco de um usuário do Azure AD, conforme determinado pela Proteção de Identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="432d1-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="432d1-106">Methods</span><span class="sxs-lookup"><span data-stu-id="432d1-106">Methods</span></span>

| <span data-ttu-id="432d1-107">Método</span><span class="sxs-lookup"><span data-stu-id="432d1-107">Method</span></span>   | <span data-ttu-id="432d1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="432d1-108">Return Type</span></span>|<span data-ttu-id="432d1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="432d1-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="432d1-110">Histórico de listas</span><span class="sxs-lookup"><span data-stu-id="432d1-110">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="432d1-111">[coleção riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="432d1-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="432d1-112">Obter o histórico de risco de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="432d1-112">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="432d1-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="432d1-113">Properties</span></span>

| <span data-ttu-id="432d1-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="432d1-114">Property</span></span>       | <span data-ttu-id="432d1-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="432d1-115">Type</span></span>    | <span data-ttu-id="432d1-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="432d1-116">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="432d1-117">userId</span><span class="sxs-lookup"><span data-stu-id="432d1-117">userId</span></span>         | <span data-ttu-id="432d1-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="432d1-118">string</span></span>  | <span data-ttu-id="432d1-119">A id do usuário.</span><span class="sxs-lookup"><span data-stu-id="432d1-119">The id of the user.</span></span> |
| <span data-ttu-id="432d1-120">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="432d1-120">initiatedBy</span></span>    | <span data-ttu-id="432d1-121">bool</span><span class="sxs-lookup"><span data-stu-id="432d1-121">bool</span></span>    | <span data-ttu-id="432d1-122">A id do ator que faz a operação.</span><span class="sxs-lookup"><span data-stu-id="432d1-122">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="432d1-123">atividade</span><span class="sxs-lookup"><span data-stu-id="432d1-123">activity</span></span>       | [<span data-ttu-id="432d1-124">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="432d1-124">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="432d1-125">A atividade relacionada à alteração no nível de risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="432d1-125">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="432d1-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="432d1-126">JSON representation</span></span>

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


