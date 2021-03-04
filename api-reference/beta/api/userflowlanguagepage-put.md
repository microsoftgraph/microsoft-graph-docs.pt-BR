---
title: Atualizar userFlowLanguagePage
description: Atualize os valores em um objeto userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2d9a38a94dfc5fe8f801a246ff4bcab2bc41eab7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433443"
---
# <a name="update-userflowlanguagepage"></a><span data-ttu-id="67529-103">Atualizar userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="67529-103">Update userFlowLanguagePage</span></span>

<span data-ttu-id="67529-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67529-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="67529-105">Atualize os valores em um objeto userFlowLanguagePage.</span><span class="sxs-lookup"><span data-stu-id="67529-105">Update the values in an userFlowLanguagePage object.</span></span> <span data-ttu-id="67529-106">Você só pode atualizar os valores em um overridesPage, que é usado para personalizar os valores mostrados a um usuário durante uma jornada do usuário definida por um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="67529-106">You may only update the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="67529-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="67529-107">Permissions</span></span>

<span data-ttu-id="67529-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67529-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67529-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67529-110">Permission type</span></span>      | <span data-ttu-id="67529-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67529-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67529-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67529-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67529-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67529-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="67529-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67529-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="67529-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67529-115">Not supported.</span></span>|
|<span data-ttu-id="67529-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67529-116">Application</span></span>|<span data-ttu-id="67529-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67529-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="67529-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="67529-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="67529-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="67529-119">Global administrator</span></span>
* <span data-ttu-id="67529-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="67529-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="67529-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67529-121">HTTP request</span></span>

<span data-ttu-id="67529-122">Para fazer referência ao conteúdo dentro do objeto, você deve usar `$value` .</span><span class="sxs-lookup"><span data-stu-id="67529-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="67529-123">Isso retorna o conteúdo dentro do objeto e permite que você o referencia diretamente.</span><span class="sxs-lookup"><span data-stu-id="67529-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
PUT /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="67529-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67529-124">Request headers</span></span>

|<span data-ttu-id="67529-125">Nome</span><span class="sxs-lookup"><span data-stu-id="67529-125">Name</span></span>|<span data-ttu-id="67529-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="67529-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="67529-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="67529-127">Authorization</span></span>|<span data-ttu-id="67529-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67529-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="67529-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67529-130">Content-Type</span></span>|<span data-ttu-id="67529-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67529-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67529-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67529-133">Request body</span></span>

<span data-ttu-id="67529-134">No corpo da solicitação, fornece uma representação JSON para os valores contidos em [um userFlowLanguagePage](../resources/userflowlanguagepage.md).</span><span class="sxs-lookup"><span data-stu-id="67529-134">In the request body, supply a JSON representation for the values contained within a [userFlowLanguagePage](../resources/userflowlanguagepage.md).</span></span>

## <a name="response"></a><span data-ttu-id="67529-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="67529-135">Response</span></span>

<span data-ttu-id="67529-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="67529-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="67529-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="67529-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67529-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67529-138">Request</span></span>

<span data-ttu-id="67529-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67529-139">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="67529-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="67529-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_overridespages"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value
Content-Type: application/json

{
  "LocalizedStrings": [
        {
            "ElementType": "UxElement",
            "ElementId": null,
            "StringId": "alert_message",
            "Override": true,
            "Value": "Are you sure that you want to cancel your selection?"
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="67529-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67529-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-overridespages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="67529-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="67529-142">Response</span></span>

<span data-ttu-id="67529-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67529-143">The following is an example of the response.</span></span>

<span data-ttu-id="67529-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="67529-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
