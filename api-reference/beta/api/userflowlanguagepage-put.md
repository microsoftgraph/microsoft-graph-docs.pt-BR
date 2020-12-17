---
title: Atualizar userFlowLanguagePage
description: Atualizar os valores em um objeto userFlowLanguagePage.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4e73897facf0407bed489a93c057c0c7f78436d5
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706245"
---
# <a name="update-userflowlanguagepage"></a><span data-ttu-id="ce0c0-103">Atualizar userFlowLanguagePage</span><span class="sxs-lookup"><span data-stu-id="ce0c0-103">Update userFlowLanguagePage</span></span>

<span data-ttu-id="ce0c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce0c0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce0c0-105">Atualizar os valores em um objeto userFlowLanguagePage.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-105">Update the values in an userFlowLanguagePage object.</span></span> <span data-ttu-id="ce0c0-106">Você só pode atualizar os valores em um overridesPage, que é usado para personalizar os valores mostrados para um usuário durante uma jornada do usuário definida por um fluxo de usuário.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-106">You may only update the values in an overridesPage, which is used to customize the values shown to a user during a user journey defined by a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce0c0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce0c0-107">Permissions</span></span>

<span data-ttu-id="ce0c0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce0c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce0c0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce0c0-110">Permission type</span></span>      | <span data-ttu-id="ce0c0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce0c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce0c0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce0c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce0c0-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce0c0-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="ce0c0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce0c0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ce0c0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-115">Not supported.</span></span>|
|<span data-ttu-id="ce0c0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce0c0-116">Application</span></span>|<span data-ttu-id="ce0c0-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce0c0-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="ce0c0-118">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="ce0c0-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="ce0c0-119">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ce0c0-119">Global administrator</span></span>
* <span data-ttu-id="ce0c0-120">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="ce0c0-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="ce0c0-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce0c0-121">HTTP request</span></span>

<span data-ttu-id="ce0c0-122">Para fazer referência ao conteúdo dentro do objeto, você deve usar `$value` .</span><span class="sxs-lookup"><span data-stu-id="ce0c0-122">To reference the content within the object, you must use `$value`.</span></span> <span data-ttu-id="ce0c0-123">Isso retorna o conteúdo dentro do objeto e permite que você faça referência a ele diretamente.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-123">This returns the content within the object and allows you to reference it directly.</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
PUT /identity/b2xUserFlows/{id}/languages/{id}/overridesPages/{id}/$value
```

## <a name="request-headers"></a><span data-ttu-id="ce0c0-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c0-124">Request headers</span></span>

|<span data-ttu-id="ce0c0-125">Nome</span><span class="sxs-lookup"><span data-stu-id="ce0c0-125">Name</span></span>|<span data-ttu-id="ce0c0-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce0c0-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ce0c0-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce0c0-127">Authorization</span></span>|<span data-ttu-id="ce0c0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce0c0-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce0c0-130">Content-Type</span></span>|<span data-ttu-id="ce0c0-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce0c0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c0-133">Request body</span></span>

<span data-ttu-id="ce0c0-134">No corpo da solicitação, forneça uma representação JSON dos valores contidos em um [userFlowLanguagePage](../resources/userflowlanguagepage.md).</span><span class="sxs-lookup"><span data-stu-id="ce0c0-134">In the request body, supply a JSON representation for the values contained within a [userFlowLanguagePage](../resources/userflowlanguagepage.md).</span></span>

## <a name="response"></a><span data-ttu-id="ce0c0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce0c0-135">Response</span></span>

<span data-ttu-id="ce0c0-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ce0c0-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce0c0-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce0c0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce0c0-138">Request</span></span>

<span data-ttu-id="ce0c0-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-139">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="ce0c0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce0c0-140">Response</span></span>

<span data-ttu-id="ce0c0-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-141">The following is an example of the response.</span></span>

<span data-ttu-id="ce0c0-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce0c0-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
