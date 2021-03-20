---
title: Criar usuário custodiadoSource
description: Crie um novo objeto userSource custodiante.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1fb67377785a8120bb6e4b1453901b9f8b0137ed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946111"
---
# <a name="create-custodian-usersource"></a><span data-ttu-id="6dc47-103">Criar usuário custodiadoSource</span><span class="sxs-lookup"><span data-stu-id="6dc47-103">Create custodian userSource</span></span>

<span data-ttu-id="6dc47-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="6dc47-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dc47-105">Crie um novo objeto [userSource](../resources/ediscovery-usersource.md) custodiante.</span><span class="sxs-lookup"><span data-stu-id="6dc47-105">Create a new custodian [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dc47-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6dc47-106">Permissions</span></span>

<span data-ttu-id="6dc47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dc47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dc47-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dc47-109">Permission type</span></span>|<span data-ttu-id="6dc47-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dc47-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dc47-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dc47-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dc47-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dc47-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="6dc47-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dc47-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dc47-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dc47-114">Not supported.</span></span>|
|<span data-ttu-id="6dc47-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dc47-115">Application</span></span>|<span data-ttu-id="6dc47-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6dc47-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dc47-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dc47-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="6dc47-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dc47-118">Request headers</span></span>

|<span data-ttu-id="6dc47-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6dc47-119">Name</span></span>|<span data-ttu-id="6dc47-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc47-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6dc47-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dc47-121">Authorization</span></span>|<span data-ttu-id="6dc47-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dc47-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6dc47-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6dc47-124">Content-Type</span></span>|<span data-ttu-id="6dc47-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dc47-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dc47-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dc47-127">Request body</span></span>

<span data-ttu-id="6dc47-128">No corpo da solicitação, fornece uma representação JSON do [objeto userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="6dc47-128">In the request body, supply a JSON representation of the [userSource](../resources/ediscovery-usersource.md) object.</span></span>

<span data-ttu-id="6dc47-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userSource](../resources/ediscovery-usersource.md).</span><span class="sxs-lookup"><span data-stu-id="6dc47-129">The following table shows the properties that are required when you create the [userSource](../resources/ediscovery-usersource.md).</span></span>

|<span data-ttu-id="6dc47-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6dc47-130">Property</span></span>|<span data-ttu-id="6dc47-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dc47-131">Type</span></span>|<span data-ttu-id="6dc47-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dc47-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dc47-133">email</span><span class="sxs-lookup"><span data-stu-id="6dc47-133">email</span></span>|<span data-ttu-id="6dc47-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6dc47-134">String</span></span>|<span data-ttu-id="6dc47-135">Endereço SMTP do usuário.</span><span class="sxs-lookup"><span data-stu-id="6dc47-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="6dc47-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="6dc47-136">includedSources</span></span>|<span data-ttu-id="6dc47-137">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="6dc47-137">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="6dc47-138">Especifica quais fontes estão incluídas neste grupo.</span><span class="sxs-lookup"><span data-stu-id="6dc47-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="6dc47-139">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="6dc47-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="6dc47-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dc47-140">Response</span></span>

<span data-ttu-id="6dc47-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dc47-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6dc47-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6dc47-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dc47-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dc47-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6dc47-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dc47-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_usersource_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
Content-Type: application/json
Content-length: 233

{
    "email":"megan@contoso.com",
    "includedSources":"mailbox, site"
}
```
# <a name="c"></a>[<span data-ttu-id="6dc47-145">C#</span><span class="sxs-lookup"><span data-stu-id="6dc47-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6dc47-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dc47-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6dc47-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dc47-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6dc47-148">Java</span><span class="sxs-lookup"><span data-stu-id="6dc47-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="6dc47-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dc47-149">Response</span></span>

<span data-ttu-id="6dc47-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6dc47-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.userSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('45454331323337443946343043464239')/userSources/$entity",
    "displayName": "Megan Bowen",
    "createdDateTime": "2020-11-06T16:09:08.4905571Z",
    "id": "34383036-3741-4545-3242-373530353435",
    "email": "megan@contoso.com",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null
        }
    }
}
```
