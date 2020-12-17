---
title: Excluir userFlowLanguagePage
description: Exclui os valores em um objeto userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 22efb148458c20709c58bde0ea9b198566912a41
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706247"
---
# <a name="delete-userflowlanguagepage"></a><span data-ttu-id="60d7f-103">Excluir userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="60d7f-103">Delete userFlowLanguagePage</span></span>

<span data-ttu-id="60d7f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60d7f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60d7f-105">Exclui os valores em um objeto [userFlowLanguagePage](../resources/userflowlanguagepage.md) .</span><span class="sxs-lookup"><span data-stu-id="60d7f-105">Deletes the values in an [userFlowLanguagePage](../resources/userflowlanguagepage.md) object.</span></span> <span data-ttu-id="60d7f-106">Você só pode excluir os valores em um overridesPage, que é usado para personalizar os valores mostrados para um usuário durante uma jornada do usuário definida por um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="60d7f-106">You may only delete the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="60d7f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="60d7f-107">Permissions</span></span>

<span data-ttu-id="60d7f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60d7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60d7f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60d7f-110">Permission type</span></span>      | <span data-ttu-id="60d7f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60d7f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60d7f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60d7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60d7f-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d7f-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="60d7f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60d7f-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="60d7f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60d7f-115">Not supported.</span></span>|
|<span data-ttu-id="60d7f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60d7f-116">Application</span></span>|<span data-ttu-id="60d7f-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d7f-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="60d7f-118">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="60d7f-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="60d7f-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="60d7f-119">Global administrator</span></span>
* <span data-ttu-id="60d7f-120">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="60d7f-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="60d7f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60d7f-121">HTTP request</span></span>

<span data-ttu-id="60d7f-122">Para fazer referência ao conteúdo dentro do objeto, você deve usar `$value` .</span><span class="sxs-lookup"><span data-stu-id="60d7f-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="60d7f-123">Isso retorna o conteúdo dentro do objeto e permite que você faça referência a ele diretamente.</span><span class="sxs-lookup"><span data-stu-id="60d7f-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/$value
DELETE /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/$value
```

## <a name="request-headers"></a><span data-ttu-id="60d7f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60d7f-124">Request headers</span></span>

|<span data-ttu-id="60d7f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="60d7f-125">Name</span></span>|<span data-ttu-id="60d7f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="60d7f-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="60d7f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="60d7f-127">Authorization</span></span>|<span data-ttu-id="60d7f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60d7f-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60d7f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60d7f-130">Request body</span></span>

<span data-ttu-id="60d7f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60d7f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60d7f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="60d7f-132">Response</span></span>

<span data-ttu-id="60d7f-133">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="60d7f-133">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="60d7f-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="60d7f-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60d7f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60d7f-135">Request</span></span>

<span data-ttu-id="60d7f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60d7f-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguagepage"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/overridesPages/phonefactor/$value
```

### <a name="response"></a><span data-ttu-id="60d7f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="60d7f-137">Response</span></span>

<span data-ttu-id="60d7f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60d7f-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
