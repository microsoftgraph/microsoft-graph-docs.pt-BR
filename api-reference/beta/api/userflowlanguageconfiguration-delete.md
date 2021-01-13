---
title: Excluir userFlowLanguageConfiguration
description: Exclui um objeto userFlowLanguageConfiguration de um fluxo de usuário B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b9a59c8786fa27b458fd6f1236a30e33f1fb355
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844946"
---
# <a name="delete-userflowlanguageconfiguration"></a><span data-ttu-id="ee0f1-103">Excluir userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee0f1-103">Delete userFlowLanguageConfiguration</span></span>

<span data-ttu-id="ee0f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee0f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee0f1-105">Exclui um [objeto userFlowLanguageConfiguration de](../resources/userflowlanguageconfiguration.md) um fluxo de usuário do [Azure AD B2C.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="ee0f1-105">Deletes a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object from a [Azure AD B2C user flow](../resources/b2cidentityuserflow.md).</span></span>

<span data-ttu-id="ee0f1-106">**Observação:** Você não pode excluir idiomas de um fluxo de usuário do [Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="ee0f1-106">**Note:** You cannot delete languages from an [Azure Active Directory user flow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ee0f1-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ee0f1-107">Permissions</span></span>

<span data-ttu-id="ee0f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee0f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee0f1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee0f1-110">Permission type</span></span>      | <span data-ttu-id="ee0f1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee0f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee0f1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee0f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee0f1-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee0f1-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ee0f1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee0f1-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ee0f1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee0f1-115">Not supported.</span></span>|
|<span data-ttu-id="ee0f1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee0f1-116">Application</span></span>|<span data-ttu-id="ee0f1-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee0f1-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ee0f1-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ee0f1-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ee0f1-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ee0f1-119">Global administrator</span></span>
* <span data-ttu-id="ee0f1-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="ee0f1-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ee0f1-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee0f1-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ee0f1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee0f1-122">Request headers</span></span>

|<span data-ttu-id="ee0f1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ee0f1-123">Name</span></span>|<span data-ttu-id="ee0f1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee0f1-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ee0f1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee0f1-125">Authorization</span></span>|<span data-ttu-id="ee0f1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee0f1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee0f1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee0f1-128">Request body</span></span>

<span data-ttu-id="ee0f1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee0f1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee0f1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee0f1-130">Response</span></span>

<span data-ttu-id="ee0f1-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ee0f1-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ee0f1-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ee0f1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee0f1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee0f1-133">Request</span></span>

<span data-ttu-id="ee0f1-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ee0f1-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee0f1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee0f1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguageconfiguration"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES
```
# <a name="c"></a>[<span data-ttu-id="ee0f1-136">C#</span><span class="sxs-lookup"><span data-stu-id="ee0f1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowlanguageconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee0f1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee0f1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowlanguageconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee0f1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee0f1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowlanguageconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee0f1-139">Java</span><span class="sxs-lookup"><span data-stu-id="ee0f1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowlanguageconfiguration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee0f1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee0f1-140">Response</span></span>

<span data-ttu-id="ee0f1-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ee0f1-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
