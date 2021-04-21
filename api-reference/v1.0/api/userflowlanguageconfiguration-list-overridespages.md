---
title: Lista substituiPages
description: Obter os recursos userFlowLanguagePage da propriedade de navegação overridesPages.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 70207f30e824f584f3e55a4ae9038bd64e840d27
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920529"
---
# <a name="list-overridespages"></a><span data-ttu-id="f6bb6-103">Lista substituiPages</span><span class="sxs-lookup"><span data-stu-id="f6bb6-103">List overridesPages</span></span>

<span data-ttu-id="f6bb6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6bb6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6bb6-105">Obter os recursos userFlowLanguagePage da propriedade de navegação overridesPages.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-105">Get the userFlowLanguagePage resources from the overridesPages navigation property.</span></span> <span data-ttu-id="f6bb6-106">Essas páginas são usadas para personalizar os valores mostrados ao usuário durante uma jornada do usuário em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-106">These pages are used to customize the values shown to the user during a user journey in a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6bb6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6bb6-107">Permissions</span></span>

<span data-ttu-id="f6bb6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6bb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6bb6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6bb6-110">Permission type</span></span>      | <span data-ttu-id="f6bb6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6bb6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6bb6-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6bb6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6bb6-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bb6-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="f6bb6-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6bb6-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="f6bb6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-115">Not supported.</span></span>|
|<span data-ttu-id="f6bb6-116">Application</span><span class="sxs-lookup"><span data-stu-id="f6bb6-116">Application</span></span>|<span data-ttu-id="f6bb6-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6bb6-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="f6bb6-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="f6bb6-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f6bb6-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f6bb6-119">Global administrator</span></span>
* <span data-ttu-id="f6bb6-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="f6bb6-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f6bb6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6bb6-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages/{id}/overridesPages
```

## <a name="request-headers"></a><span data-ttu-id="f6bb6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bb6-122">Request headers</span></span>

|<span data-ttu-id="f6bb6-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f6bb6-123">Name</span></span>|<span data-ttu-id="f6bb6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6bb6-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6bb6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6bb6-125">Authorization</span></span>|<span data-ttu-id="f6bb6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6bb6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bb6-128">Request body</span></span>

<span data-ttu-id="f6bb6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6bb6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6bb6-130">Response</span></span>

<span data-ttu-id="f6bb6-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos userFlowLanguagePage](../resources/userflowlanguagepage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6bb6-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f6bb6-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6bb6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6bb6-133">Request</span></span>

<span data-ttu-id="f6bb6-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f6bb6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6bb6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_2"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en/overridesPages
```
# <a name="c"></a>[<span data-ttu-id="f6bb6-136">C#</span><span class="sxs-lookup"><span data-stu-id="f6bb6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6bb6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6bb6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6bb6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6bb6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6bb6-139">Java</span><span class="sxs-lookup"><span data-stu-id="f6bb6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f6bb6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6bb6-140">Response</span></span>

<span data-ttu-id="f6bb6-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-141">The following is an example of the response.</span></span>

<span data-ttu-id="f6bb6-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f6bb6-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguagePage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "selfasserted1_1"
    }
  ]
}
```
