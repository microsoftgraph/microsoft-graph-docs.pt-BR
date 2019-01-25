---
title: Atualizar contrato
description: Atualize as propriedades de um objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: fc6e4718a026f78a6e892dc13095492099b654cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520064"
---
# <a name="update-agreement"></a><span data-ttu-id="6c79a-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="6c79a-103">Update agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c79a-104">Atualize as propriedades de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="6c79a-104">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6c79a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c79a-105">Permissions</span></span>
<span data-ttu-id="6c79a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c79a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c79a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c79a-108">Permission type</span></span>                        | <span data-ttu-id="6c79a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c79a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c79a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c79a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c79a-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c79a-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="6c79a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c79a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c79a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c79a-113">Not supported.</span></span> |
|<span data-ttu-id="6c79a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c79a-114">Application</span></span>                            | <span data-ttu-id="6c79a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c79a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c79a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c79a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="6c79a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c79a-117">Request headers</span></span>
| <span data-ttu-id="6c79a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6c79a-118">Name</span></span>         | <span data-ttu-id="6c79a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c79a-119">Type</span></span>        | <span data-ttu-id="6c79a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c79a-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6c79a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c79a-121">Authorization</span></span> | <span data-ttu-id="6c79a-122">string</span><span class="sxs-lookup"><span data-stu-id="6c79a-122">string</span></span> | <span data-ttu-id="6c79a-123">Token de portador</span><span class="sxs-lookup"><span data-stu-id="6c79a-123">Bearer \{token\}.</span></span> <span data-ttu-id="6c79a-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c79a-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c79a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c79a-125">Request body</span></span>
<span data-ttu-id="6c79a-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6c79a-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6c79a-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6c79a-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6c79a-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6c79a-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6c79a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c79a-129">Property</span></span>     | <span data-ttu-id="6c79a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c79a-130">Type</span></span>        | <span data-ttu-id="6c79a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c79a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c79a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6c79a-132">displayName</span></span>|<span data-ttu-id="6c79a-133">String</span><span class="sxs-lookup"><span data-stu-id="6c79a-133">String</span></span>|<span data-ttu-id="6c79a-134">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="6c79a-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="6c79a-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="6c79a-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="6c79a-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c79a-136">Boolean</span></span>|<span data-ttu-id="6c79a-137">Se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="6c79a-137">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="6c79a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c79a-138">Response</span></span>
<span data-ttu-id="6c79a-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [contrato](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c79a-139">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c79a-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c79a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c79a-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c79a-141">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/beta/agreements/<id>
Content-type: application/json
Content-length: 85

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="6c79a-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c79a-142">Response</span></span>
><span data-ttu-id="6c79a-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c79a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 105

{
  "displayName": "displayName-value",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
