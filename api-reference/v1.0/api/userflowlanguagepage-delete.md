---
title: Excluir userFlowLanguagePage
description: Exclui os valores em um objeto userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 791c43817d9a8f8e8369e4d0d8adf5eb0a75580a
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882851"
---
# <a name="delete-userflowlanguagepage"></a><span data-ttu-id="6032a-103">Excluir userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="6032a-103">Delete userFlowLanguagePage</span></span>

<span data-ttu-id="6032a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6032a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6032a-105">Exclui os valores em um [objeto userFlowLanguagePage.](../resources/userflowlanguagepage.md)</span><span class="sxs-lookup"><span data-stu-id="6032a-105">Deletes the values in an [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span> <span data-ttu-id="6032a-106">Você só pode excluir os valores em um overridesPage, que é usado para personalizar os valores mostrados a um usuário durante uma jornada do usuário definida por um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="6032a-106">You may only delete the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="6032a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6032a-107">Permissions</span></span>

<span data-ttu-id="6032a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6032a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6032a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6032a-110">Permission type</span></span>      | <span data-ttu-id="6032a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6032a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6032a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6032a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6032a-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6032a-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="6032a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6032a-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6032a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6032a-115">Not supported.</span></span>|
|<span data-ttu-id="6032a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6032a-116">Application</span></span>|<span data-ttu-id="6032a-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6032a-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="6032a-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="6032a-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="6032a-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6032a-119">Global administrator</span></span>
* <span data-ttu-id="6032a-120">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="6032a-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="6032a-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6032a-121">HTTP request</span></span>

<span data-ttu-id="6032a-122">Para fazer referência ao conteúdo dentro do objeto, você deve usar `$value` .</span><span class="sxs-lookup"><span data-stu-id="6032a-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="6032a-123">Isso retorna o conteúdo dentro do objeto e permite que você o referencia diretamente.</span><span class="sxs-lookup"><span data-stu-id="6032a-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a><span data-ttu-id="6032a-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6032a-124">Request headers</span></span>

|<span data-ttu-id="6032a-125">Nome</span><span class="sxs-lookup"><span data-stu-id="6032a-125">Name</span></span>|<span data-ttu-id="6032a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6032a-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6032a-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6032a-127">Authorization</span></span>|<span data-ttu-id="6032a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6032a-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6032a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6032a-130">Request body</span></span>

<span data-ttu-id="6032a-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6032a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6032a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6032a-132">Response</span></span>

<span data-ttu-id="6032a-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6032a-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6032a-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6032a-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6032a-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6032a-135">Request</span></span>

<span data-ttu-id="6032a-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6032a-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2X_1_Partner/languages/en/overridesPages/selfasserted1_1/$value
```

### <a name="response"></a><span data-ttu-id="6032a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6032a-137">Response</span></span>

<span data-ttu-id="6032a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6032a-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
