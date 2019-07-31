---
title: tipo de recurso riskyUserHistoryItem
description: Representa o histórico de riscos de usuários do Azure AD
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 586fdb046adc8977550cc386a27284752cf487c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965331"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="f55b5-103">tipo de recurso riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="f55b5-103">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="f55b5-104">Representa o histórico de riscos de um usuário do Azure AD, conforme determinado pela proteção de identidade do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f55b5-104">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span> 

## <a name="methods"></a><span data-ttu-id="f55b5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f55b5-105">Methods</span></span>

| <span data-ttu-id="f55b5-106">Método</span><span class="sxs-lookup"><span data-stu-id="f55b5-106">Method</span></span>   | <span data-ttu-id="f55b5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f55b5-107">Return Type</span></span>|<span data-ttu-id="f55b5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f55b5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f55b5-109">Histórico de lista</span><span class="sxs-lookup"><span data-stu-id="f55b5-109">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="f55b5-110">coleção [riskyUserHistoryItem](riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f55b5-110">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="f55b5-111">Obter o histórico de riscos de um usuário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f55b5-111">Get the risk history of an Azure AD user.</span></span>|


## <a name="properties"></a><span data-ttu-id="f55b5-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f55b5-112">Properties</span></span>

| <span data-ttu-id="f55b5-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f55b5-113">Property</span></span>       | <span data-ttu-id="f55b5-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="f55b5-114">Type</span></span>    | <span data-ttu-id="f55b5-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="f55b5-115">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="f55b5-116">userId</span><span class="sxs-lookup"><span data-stu-id="f55b5-116">userId</span></span>         | <span data-ttu-id="f55b5-117">string</span><span class="sxs-lookup"><span data-stu-id="f55b5-117">string</span></span>  | <span data-ttu-id="f55b5-118">A ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="f55b5-118">The id of the user.</span></span> |
| <span data-ttu-id="f55b5-119">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="f55b5-119">initiatedBy</span></span>    | <span data-ttu-id="f55b5-120">bool</span><span class="sxs-lookup"><span data-stu-id="f55b5-120">bool</span></span>    | <span data-ttu-id="f55b5-121">A ID do ator que faz a operação.</span><span class="sxs-lookup"><span data-stu-id="f55b5-121">The id of actor that does the operation.</span></span> |
| <span data-ttu-id="f55b5-122">atividade</span><span class="sxs-lookup"><span data-stu-id="f55b5-122">activity</span></span>       | [<span data-ttu-id="f55b5-123">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="f55b5-123">riskUserActivity</span></span>](riskuseractivity.md)| <span data-ttu-id="f55b5-124">A atividade relacionada à alteração no nível de risco do usuário.</span><span class="sxs-lookup"><span data-stu-id="f55b5-124">The activity related to user risk level change.</span></span> | 

## <a name="json-representation"></a><span data-ttu-id="f55b5-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f55b5-125">JSON representation</span></span>

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
