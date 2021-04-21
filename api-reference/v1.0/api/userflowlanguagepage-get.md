---
title: Obter userFlowLanguagePage
description: Leia os valores em um objeto userFlowLanguagePage para um idioma em um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bf35e829e0c5f8cc9df6af502962aab4a6a4a83b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920460"
---
# <a name="get-userflowlanguagepage"></a><span data-ttu-id="91575-103">Obter userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="91575-103">Get userFlowLanguagePage</span></span>

<span data-ttu-id="91575-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91575-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91575-105">Leia os valores em [um objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) para um idioma em um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="91575-105">Read the values in a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object for a language in a user flow.</span></span> <span data-ttu-id="91575-106">Esses valores são mostrados a um usuário durante uma jornada do usuário definida por um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="91575-106">These values are shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="91575-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="91575-107">Permissions</span></span>

<span data-ttu-id="91575-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91575-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91575-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91575-110">Permission type</span></span>      | <span data-ttu-id="91575-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91575-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91575-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91575-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91575-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91575-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="91575-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91575-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="91575-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91575-115">Not supported.</span></span>|
|<span data-ttu-id="91575-116">Application</span><span class="sxs-lookup"><span data-stu-id="91575-116">Application</span></span>|<span data-ttu-id="91575-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91575-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="91575-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="91575-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="91575-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="91575-119">Global administrator</span></span>
* <span data-ttu-id="91575-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="91575-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="91575-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91575-121">HTTP request</span></span>

<span data-ttu-id="91575-122">Para fazer referência ao conteúdo dentro do objeto, você deve usar `$value` .</span><span class="sxs-lookup"><span data-stu-id="91575-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="91575-123">Isso retorna o conteúdo dentro do objeto e permite que você o referencia diretamente.</span><span class="sxs-lookup"><span data-stu-id="91575-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages/{id}/$value
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="91575-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91575-124">Request headers</span></span>

|<span data-ttu-id="91575-125">Nome</span><span class="sxs-lookup"><span data-stu-id="91575-125">Name</span></span>|<span data-ttu-id="91575-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="91575-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="91575-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="91575-127">Authorization</span></span>|<span data-ttu-id="91575-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91575-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="91575-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91575-130">Request body</span></span>

<span data-ttu-id="91575-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91575-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91575-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="91575-132">Response</span></span>

<span data-ttu-id="91575-133">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userFlowLanguagePage](../resources/userflowlanguagepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91575-133">If successful, this method returns a `200 OK` response code and a [userFlowLanguagePage](../resources/userflowlanguagepage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="91575-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="91575-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="91575-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91575-135">Request</span></span>

<span data-ttu-id="91575-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="91575-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="91575-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="91575-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en/defaultPages/idpselections/$value
```
# <a name="c"></a>[<span data-ttu-id="91575-138">C#</span><span class="sxs-lookup"><span data-stu-id="91575-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91575-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91575-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91575-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91575-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91575-141">Java</span><span class="sxs-lookup"><span data-stu-id="91575-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="91575-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="91575-142">Response</span></span>

<span data-ttu-id="91575-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="91575-143">The following is an example of the response.</span></span>

<span data-ttu-id="91575-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="91575-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguagePage"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "LocalizedStrings": [
      {
        "ElementType": "ErrorMessage",
        "ElementId": null,
        "StringId": "ServiceThrottled",
        "Override": false,
        "Value": "There are too many requests at this moment. Please wait for some time and try again."
      }
   ]
}
```
