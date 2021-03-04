---
title: Criar custodiatário
description: Crie um novo objeto custodiante.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 80c3a8f6bb7a204ddc5512d1f6c66b261ea342a6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445829"
---
# <a name="create-custodian"></a><span data-ttu-id="f05f3-103">Criar custodiatário</span><span class="sxs-lookup"><span data-stu-id="f05f3-103">Create custodian</span></span>

<span data-ttu-id="f05f3-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f05f3-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f05f3-105">Crie um novo [objeto custodiante.](../resources/ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="f05f3-105">Create a new [custodian](../resources/ediscovery-custodian.md) object.</span></span> <span data-ttu-id="f05f3-106">Depois que o objeto custodiante for criado, você precisará criar o [usuário do custodianteSource](../resources/ediscovery-usersource.md) para fazer referência à caixa de correio e ao site do OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="f05f3-106">After the custodian object is created, you will need to create the custodian's [userSource](../resources/ediscovery-usersource.md) to reference their mailbox and OneDrive for Business site.</span></span>

## <a name="permissions"></a><span data-ttu-id="f05f3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f05f3-107">Permissions</span></span>

<span data-ttu-id="f05f3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f05f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f05f3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f05f3-110">Permission type</span></span>|<span data-ttu-id="f05f3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f05f3-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f05f3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f05f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f05f3-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f05f3-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f05f3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f05f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f05f3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f05f3-115">Not supported.</span></span>|
|<span data-ttu-id="f05f3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f05f3-116">Application</span></span>|<span data-ttu-id="f05f3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f05f3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f05f3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f05f3-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians
```

## <a name="request-headers"></a><span data-ttu-id="f05f3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f05f3-119">Request headers</span></span>

|<span data-ttu-id="f05f3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f05f3-120">Name</span></span>|<span data-ttu-id="f05f3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f05f3-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f05f3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f05f3-122">Authorization</span></span>|<span data-ttu-id="f05f3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f05f3-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f05f3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f05f3-125">Content-Type</span></span>|<span data-ttu-id="f05f3-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f05f3-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f05f3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f05f3-128">Request body</span></span>

<span data-ttu-id="f05f3-129">No corpo da solicitação, fornece uma representação JSON do [objeto custodiante.](../resources/ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="f05f3-129">In the request body, supply a JSON representation of the [custodian](../resources/ediscovery-custodian.md) object.</span></span>

<span data-ttu-id="f05f3-130">A tabela a seguir mostra as propriedades que são necessárias ao criar [o custodiado](../resources/ediscovery-custodian.md).</span><span class="sxs-lookup"><span data-stu-id="f05f3-130">The following table shows the properties that are required when you create the [custodian](../resources/ediscovery-custodian.md).</span></span>

|<span data-ttu-id="f05f3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f05f3-131">Property</span></span>|<span data-ttu-id="f05f3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f05f3-132">Type</span></span>|<span data-ttu-id="f05f3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f05f3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f05f3-134">email</span><span class="sxs-lookup"><span data-stu-id="f05f3-134">email</span></span>|<span data-ttu-id="f05f3-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f05f3-135">String</span></span>|<span data-ttu-id="f05f3-136">O endereço SMTP principal do custodiado.</span><span class="sxs-lookup"><span data-stu-id="f05f3-136">Custodian's primary SMTP address.</span></span> <span data-ttu-id="f05f3-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f05f3-137">Required.</span></span>|
|<span data-ttu-id="f05f3-138">applyHoldToSources</span><span class="sxs-lookup"><span data-stu-id="f05f3-138">applyHoldToSources</span></span>|<span data-ttu-id="f05f3-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="f05f3-139">Boolean</span></span>|<span data-ttu-id="f05f3-140">Indica se uma união é aplicada às fontes do custodiante (como caixas de correio, sites ou Teams).</span><span class="sxs-lookup"><span data-stu-id="f05f3-140">Indicates whether a hold is applied to the custodian's sources (such as mailboxes, sites, or Teams).</span></span>|

## <a name="response"></a><span data-ttu-id="f05f3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05f3-141">Response</span></span>

<span data-ttu-id="f05f3-142">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f05f3-142">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f05f3-143">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f05f3-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f05f3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f05f3-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f05f3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f05f3-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_custodian_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
Content-Type: application/json
Content-length: 279

{
    "email":"AdeleV@contoso.com",
    "applyHoldToSources":"true"
}
```

# <a name="c"></a>[<span data-ttu-id="f05f3-146">C#</span><span class="sxs-lookup"><span data-stu-id="f05f3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-custodian-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f05f3-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f05f3-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-custodian-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f05f3-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f05f3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-custodian-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f05f3-149">Java</span><span class="sxs-lookup"><span data-stu-id="f05f3-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-custodian-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f05f3-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f05f3-150">Response</span></span>

<span data-ttu-id="f05f3-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f05f3-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.custodian"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:47:01.7724531Z",
    "lastModifiedDateTime": "2020-10-30T20:47:02.2512381Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45353243323138344430413038363846",
    "displayName": "Adele Vance"
}
```
