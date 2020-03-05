---
title: tipo de recurso riskyUserHistoryItem
description: Representa o histórico de riscos de usuários do Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 519e2a7fdb6662496cdb660095ec63ce81b849f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521051"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="85149-103">tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="85149-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="85149-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="85149-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="85149-105">Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85149-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="85149-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="85149-106">Methods</span></span>

| <span data-ttu-id="85149-107">Método</span><span class="sxs-lookup"><span data-stu-id="85149-107">Method</span></span>   | <span data-ttu-id="85149-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="85149-108">Return Type</span></span>|<span data-ttu-id="85149-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="85149-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85149-110">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="85149-110">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="85149-111">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="85149-111">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="85149-112">Obter o histórico de riscos de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="85149-112">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="85149-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85149-113">Properties</span></span>

| <span data-ttu-id="85149-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85149-114">Property</span></span>       | <span data-ttu-id="85149-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="85149-115">Type</span></span>    | <span data-ttu-id="85149-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="85149-116">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="85149-117">userId</span><span class="sxs-lookup"><span data-stu-id="85149-117">userId</span></span>         | <span data-ttu-id="85149-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85149-118">string</span></span>  | <span data-ttu-id="85149-119">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="85149-119">The id of the user.</span></span> |
| <span data-ttu-id="85149-120">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="85149-120">initiatedBy</span></span>    | <span data-ttu-id="85149-121">bool</span><span class="sxs-lookup"><span data-stu-id="85149-121">bool</span></span>    | <span data-ttu-id="85149-122">A ID do ator que faz a operação.</span><span class="sxs-lookup"><span data-stu-id="85149-122">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="85149-123">atividade</span><span class="sxs-lookup"><span data-stu-id="85149-123">activity</span></span>       | [<span data-ttu-id="85149-124">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="85149-124">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="85149-125">A atividade relacionada à alteração no nível de risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="85149-125">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="85149-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85149-126">JSON representation</span></span>

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
