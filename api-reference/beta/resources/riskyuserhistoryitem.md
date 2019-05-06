---
title: tipo de recurso riskyUserHistoryItem
description: Representa o histórico de riscos de usuários do Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37f38a649aa3721e65b44e64571dafb797259cf6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33620833"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="53ac4-103">tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="53ac4-103">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="53ac4-104">Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="53ac4-104">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="53ac4-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="53ac4-105">Methods</span></span>

| <span data-ttu-id="53ac4-106">Método</span><span class="sxs-lookup"><span data-stu-id="53ac4-106">Method</span></span>   | <span data-ttu-id="53ac4-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="53ac4-107">Return Type</span></span>|<span data-ttu-id="53ac4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="53ac4-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="53ac4-109">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="53ac4-109">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="53ac4-110">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="53ac4-110">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="53ac4-111">Obter o histórico de riscos de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="53ac4-111">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="53ac4-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53ac4-112">Properties</span></span>

| <span data-ttu-id="53ac4-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53ac4-113">Property</span></span>       | <span data-ttu-id="53ac4-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="53ac4-114">Type</span></span>    | <span data-ttu-id="53ac4-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="53ac4-115">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="53ac4-116">userId</span><span class="sxs-lookup"><span data-stu-id="53ac4-116">userId</span></span>         | <span data-ttu-id="53ac4-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53ac4-117">string</span></span>  | <span data-ttu-id="53ac4-118">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="53ac4-118">The id of the user.</span></span> |
| <span data-ttu-id="53ac4-119">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="53ac4-119">initiatedBy</span></span>    | <span data-ttu-id="53ac4-120">bool</span><span class="sxs-lookup"><span data-stu-id="53ac4-120">bool</span></span>    | <span data-ttu-id="53ac4-121">A ID do ator que faz a operação.</span><span class="sxs-lookup"><span data-stu-id="53ac4-121">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="53ac4-122">atividade</span><span class="sxs-lookup"><span data-stu-id="53ac4-122">activity</span></span>       | [<span data-ttu-id="53ac4-123">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="53ac4-123">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="53ac4-124">A atividade relacionada à alteração no nível de risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="53ac4-124">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="53ac4-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53ac4-125">JSON representation</span></span>

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
