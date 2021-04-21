---
title: Obter userFlowLanguageConfiguration
description: Leia as propriedades e as relações de um objeto userFlowLanguageConfiguration.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a2f17c309e104738a1bae4fd7e599fd8efa28355
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920566"
---
# <a name="get-userflowlanguageconfiguration"></a><span data-ttu-id="47d31-103">Obter userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="47d31-103">Get userFlowLanguageConfiguration</span></span>

<span data-ttu-id="47d31-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47d31-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47d31-105">Leia as propriedades e as relações de um [objeto userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47d31-105">Read the properties and relationships of a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span> <span data-ttu-id="47d31-106">Esses objetos representam um idioma disponível em um fluxo de usuários.</span><span class="sxs-lookup"><span data-stu-id="47d31-106">These objects represent a language available in a user flow.</span></span>

<span data-ttu-id="47d31-107">**Observação:** A personalização de idioma é habilitada por padrão nos fluxos de [usuários do Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="47d31-107">**Note:** Language customization is enabled by default in [Azure Active Directory user flows](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="47d31-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="47d31-108">Permissions</span></span>

<span data-ttu-id="47d31-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47d31-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47d31-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47d31-111">Permission type</span></span>      | <span data-ttu-id="47d31-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47d31-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47d31-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47d31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47d31-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d31-114">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="47d31-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47d31-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="47d31-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47d31-116">Not supported.</span></span>|
|<span data-ttu-id="47d31-117">Application</span><span class="sxs-lookup"><span data-stu-id="47d31-117">Application</span></span>|<span data-ttu-id="47d31-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d31-118">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="47d31-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="47d31-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="47d31-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="47d31-120">Global administrator</span></span>
* <span data-ttu-id="47d31-121">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="47d31-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="47d31-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47d31-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET identity/b2xUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="47d31-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47d31-123">Request headers</span></span>

|<span data-ttu-id="47d31-124">Nome</span><span class="sxs-lookup"><span data-stu-id="47d31-124">Name</span></span>|<span data-ttu-id="47d31-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="47d31-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47d31-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="47d31-126">Authorization</span></span>|<span data-ttu-id="47d31-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47d31-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d31-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47d31-129">Request body</span></span>

<span data-ttu-id="47d31-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47d31-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47d31-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="47d31-131">Response</span></span>

<span data-ttu-id="47d31-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47d31-132">If successful, this method returns a `200 OK` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47d31-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47d31-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47d31-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47d31-134">Request</span></span>

<span data-ttu-id="47d31-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="47d31-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47d31-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="47d31-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/languages/en
```
# <a name="c"></a>[<span data-ttu-id="47d31-137">C#</span><span class="sxs-lookup"><span data-stu-id="47d31-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47d31-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47d31-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47d31-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47d31-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47d31-140">Java</span><span class="sxs-lookup"><span data-stu-id="47d31-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47d31-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="47d31-141">Response</span></span>

<span data-ttu-id="47d31-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="47d31-142">The following is an example of the response.</span></span>

<span data-ttu-id="47d31-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47d31-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_Partner')/languages/$entity",
    "id": "en",
    "isEnabled": true,
    "displayName": "English"
  }
}
```
