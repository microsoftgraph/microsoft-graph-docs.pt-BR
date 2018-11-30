---
title: Atualizar contrato
description: Atualize as propriedades de um objeto de contrato.
ms.openlocfilehash: b9405a8c469876a349b5c1b0c00e6f6a5f225e72
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034075"
---
# <a name="update-agreement"></a><span data-ttu-id="1fea3-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="1fea3-103">Update agreement</span></span>

> <span data-ttu-id="1fea3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1fea3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fea3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1fea3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1fea3-106">Atualize as propriedades de um objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="1fea3-106">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1fea3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1fea3-107">Permissions</span></span>
<span data-ttu-id="1fea3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fea3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fea3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fea3-110">Permission type</span></span>                        | <span data-ttu-id="1fea3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fea3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fea3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fea3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fea3-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fea3-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="1fea3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fea3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fea3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fea3-115">Not supported.</span></span> |
|<span data-ttu-id="1fea3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fea3-116">Application</span></span>                            | <span data-ttu-id="1fea3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fea3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fea3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fea3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /agreements/<id>
```
## <a name="request-headers"></a><span data-ttu-id="1fea3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fea3-119">Request headers</span></span>
| <span data-ttu-id="1fea3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1fea3-120">Name</span></span>         | <span data-ttu-id="1fea3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fea3-121">Type</span></span>        | <span data-ttu-id="1fea3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fea3-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1fea3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fea3-123">Authorization</span></span> | <span data-ttu-id="1fea3-124">string</span><span class="sxs-lookup"><span data-stu-id="1fea3-124">string</span></span> | <span data-ttu-id="1fea3-125">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="1fea3-125">Bearer \{token\}.</span></span> <span data-ttu-id="1fea3-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fea3-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fea3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fea3-127">Request body</span></span>
<span data-ttu-id="1fea3-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="1fea3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1fea3-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="1fea3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1fea3-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1fea3-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1fea3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fea3-131">Property</span></span>     | <span data-ttu-id="1fea3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fea3-132">Type</span></span>        | <span data-ttu-id="1fea3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fea3-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1fea3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1fea3-134">displayName</span></span>|<span data-ttu-id="1fea3-135">String</span><span class="sxs-lookup"><span data-stu-id="1fea3-135">String</span></span>|<span data-ttu-id="1fea3-136">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="1fea3-136">Display name of the agreement.</span></span>|
|<span data-ttu-id="1fea3-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="1fea3-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="1fea3-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fea3-138">Boolean</span></span>|<span data-ttu-id="1fea3-139">Se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="1fea3-139">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="1fea3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fea3-140">Response</span></span>
<span data-ttu-id="1fea3-141">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [contrato](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fea3-141">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1fea3-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fea3-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fea3-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fea3-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="1fea3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fea3-144">Response</span></span>
><span data-ttu-id="1fea3-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fea3-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
