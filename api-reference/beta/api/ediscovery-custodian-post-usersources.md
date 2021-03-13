---
title: Criar usuário custodiadoSource
description: Crie um novo objeto userSource custodiante.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: bc683082d0839673b7f7f4ef4a8d4e5c41675f7e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773204"
---
# <a name="create-custodian-usersource"></a><span data-ttu-id="39726-103">Criar usuário custodiadoSource</span><span class="sxs-lookup"><span data-stu-id="39726-103">Create custodian userSource</span></span>

<span data-ttu-id="39726-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="39726-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39726-105">Crie um novo objeto [userSource](../resources/ediscovery-usersource.md) custodiante.</span><span class="sxs-lookup"><span data-stu-id="39726-105">Create a new custodian [userSource](../resources/ediscovery-usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39726-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39726-106">Permissions</span></span>

<span data-ttu-id="39726-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39726-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39726-109">Permission type</span></span>|<span data-ttu-id="39726-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39726-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39726-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39726-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39726-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39726-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="39726-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39726-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39726-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39726-114">Not supported.</span></span>|
|<span data-ttu-id="39726-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39726-115">Application</span></span>|<span data-ttu-id="39726-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39726-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39726-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39726-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="39726-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39726-118">Request headers</span></span>

|<span data-ttu-id="39726-119">Nome</span><span class="sxs-lookup"><span data-stu-id="39726-119">Name</span></span>|<span data-ttu-id="39726-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="39726-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="39726-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="39726-121">Authorization</span></span>|<span data-ttu-id="39726-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39726-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="39726-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="39726-124">Content-Type</span></span>|<span data-ttu-id="39726-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39726-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39726-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39726-127">Request body</span></span>

<span data-ttu-id="39726-128">No corpo da solicitação, fornece uma representação JSON do [objeto userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="39726-128">In the request body, supply a JSON representation of the [userSource](../resources/ediscovery-usersource.md) object.</span></span>

<span data-ttu-id="39726-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userSource](../resources/ediscovery-usersource.md).</span><span class="sxs-lookup"><span data-stu-id="39726-129">The following table shows the properties that are required when you create the [userSource](../resources/ediscovery-usersource.md).</span></span>

|<span data-ttu-id="39726-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39726-130">Property</span></span>|<span data-ttu-id="39726-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="39726-131">Type</span></span>|<span data-ttu-id="39726-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="39726-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39726-133">email</span><span class="sxs-lookup"><span data-stu-id="39726-133">email</span></span>|<span data-ttu-id="39726-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39726-134">String</span></span>|<span data-ttu-id="39726-135">Endereço SMTP do usuário.</span><span class="sxs-lookup"><span data-stu-id="39726-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="39726-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="39726-136">includedSources</span></span>|<span data-ttu-id="39726-137">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="39726-137">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="39726-138">Especifica quais fontes estão incluídas neste grupo.</span><span class="sxs-lookup"><span data-stu-id="39726-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="39726-139">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="39726-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="39726-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="39726-140">Response</span></span>

<span data-ttu-id="39726-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39726-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39726-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="39726-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39726-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39726-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39726-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="39726-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_usersource_from_"
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
# <a name="c"></a>[<span data-ttu-id="39726-145">C#</span><span class="sxs-lookup"><span data-stu-id="39726-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39726-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39726-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39726-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39726-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39726-148">Java</span><span class="sxs-lookup"><span data-stu-id="39726-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="39726-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="39726-149">Response</span></span>

<span data-ttu-id="39726-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="39726-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
