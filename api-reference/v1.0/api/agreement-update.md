---
title: Atualizar contrato
description: Atualize as propriedades de um objeto agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: d7c916e05268e4dfc2a3f080310d274ccaaa7a47
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722518"
---
# <a name="update-agreement"></a><span data-ttu-id="df4f3-103">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="df4f3-103">Update agreement</span></span>

<span data-ttu-id="df4f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df4f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df4f3-105">Atualize as propriedades de um [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="df4f3-105">Update the properties of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="df4f3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="df4f3-106">Permissions</span></span>
<span data-ttu-id="df4f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df4f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df4f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df4f3-109">Permission type</span></span>                        | <span data-ttu-id="df4f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df4f3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="df4f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df4f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df4f3-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df4f3-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="df4f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df4f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df4f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df4f3-114">Not supported.</span></span> |
|<span data-ttu-id="df4f3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df4f3-115">Application</span></span>                            | <span data-ttu-id="df4f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df4f3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="df4f3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df4f3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/termsOfUse/agreements/{id}
```
## <a name="request-headers"></a><span data-ttu-id="df4f3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df4f3-118">Request headers</span></span>
| <span data-ttu-id="df4f3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="df4f3-119">Name</span></span>         | <span data-ttu-id="df4f3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="df4f3-120">Type</span></span>        | <span data-ttu-id="df4f3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="df4f3-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="df4f3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="df4f3-122">Authorization</span></span> | <span data-ttu-id="df4f3-123">string</span><span class="sxs-lookup"><span data-stu-id="df4f3-123">string</span></span> | <span data-ttu-id="df4f3-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df4f3-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df4f3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df4f3-126">Request body</span></span>
<span data-ttu-id="df4f3-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="df4f3-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="df4f3-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="df4f3-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="df4f3-129">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="df4f3-129">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="df4f3-130">Somente as propriedades a seguir são suportadas para atualização.</span><span class="sxs-lookup"><span data-stu-id="df4f3-130">Only the following properties are supported for update.</span></span>

| <span data-ttu-id="df4f3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df4f3-131">Property</span></span>     | <span data-ttu-id="df4f3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="df4f3-132">Type</span></span>        | <span data-ttu-id="df4f3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="df4f3-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df4f3-134">displayName</span><span class="sxs-lookup"><span data-stu-id="df4f3-134">displayName</span></span>|<span data-ttu-id="df4f3-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df4f3-135">String</span></span>|<span data-ttu-id="df4f3-136">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="df4f3-136">Display name of the agreement.</span></span>|
|<span data-ttu-id="df4f3-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="df4f3-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="df4f3-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="df4f3-138">Boolean</span></span>|<span data-ttu-id="df4f3-139">Se o usuário precisa expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="df4f3-139">Whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="response"></a><span data-ttu-id="df4f3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4f3-140">Response</span></span>
<span data-ttu-id="df4f3-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto de [contrato](../resources/agreement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df4f3-141">If successful, this method returns a `200 OK` response code and an updated [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df4f3-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df4f3-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="df4f3-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df4f3-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_agreement"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be
Content-type: application/json
Content-length: 85

{
  "displayName": "Sample ToU display name",
  "isViewingBeforeAcceptanceRequired": true
}
```

### <a name="response"></a><span data-ttu-id="df4f3-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="df4f3-144">Response</span></span>
><span data-ttu-id="df4f3-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df4f3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "displayName": "Sample ToU display name",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
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
  ]
}
-->


