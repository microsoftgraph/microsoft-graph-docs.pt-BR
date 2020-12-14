---
title: Criar usuário
description: Criar um novo objeto username.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: a6aec9f8dbe7781679564c6be85cabb3ced81410
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658997"
---
# <a name="create-usersource"></a><span data-ttu-id="18dd6-103">Criar usuário</span><span class="sxs-lookup"><span data-stu-id="18dd6-103">Create userSource</span></span>

<span data-ttu-id="18dd6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18dd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18dd6-105">Criar um novo objeto [username](../resources/usersource.md) .</span><span class="sxs-lookup"><span data-stu-id="18dd6-105">Create a new [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18dd6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="18dd6-106">Permissions</span></span>

<span data-ttu-id="18dd6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18dd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18dd6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18dd6-109">Permission type</span></span>|<span data-ttu-id="18dd6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18dd6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18dd6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18dd6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18dd6-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="18dd6-112">User.Read</span></span>|
|<span data-ttu-id="18dd6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18dd6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18dd6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18dd6-114">Not supported.</span></span>|
|<span data-ttu-id="18dd6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18dd6-115">Application</span></span>|<span data-ttu-id="18dd6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18dd6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18dd6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18dd6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="18dd6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18dd6-118">Request headers</span></span>

|<span data-ttu-id="18dd6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="18dd6-119">Name</span></span>|<span data-ttu-id="18dd6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="18dd6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="18dd6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="18dd6-121">Authorization</span></span>|<span data-ttu-id="18dd6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18dd6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="18dd6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18dd6-124">Content-Type</span></span>|<span data-ttu-id="18dd6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18dd6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18dd6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18dd6-127">Request body</span></span>

<span data-ttu-id="18dd6-128">No corpo da solicitação, forneça uma representação JSON do objeto [username](../resources/usersource.md) .</span><span class="sxs-lookup"><span data-stu-id="18dd6-128">In the request body, supply a JSON representation of the [userSource](../resources/usersource.md) object.</span></span>

<span data-ttu-id="18dd6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o [username](../resources/usersource.md).</span><span class="sxs-lookup"><span data-stu-id="18dd6-129">The following table shows the properties that are required when you create the [userSource](../resources/usersource.md).</span></span>

|<span data-ttu-id="18dd6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18dd6-130">Property</span></span>|<span data-ttu-id="18dd6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18dd6-131">Type</span></span>|<span data-ttu-id="18dd6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18dd6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18dd6-133">email</span><span class="sxs-lookup"><span data-stu-id="18dd6-133">email</span></span>|<span data-ttu-id="18dd6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18dd6-134">String</span></span>|<span data-ttu-id="18dd6-135">Endereço SMTP do usuário.</span><span class="sxs-lookup"><span data-stu-id="18dd6-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="18dd6-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="18dd6-136">includedSources</span></span>|<span data-ttu-id="18dd6-137">sourceType</span><span class="sxs-lookup"><span data-stu-id="18dd6-137">sourceType</span></span>|<span data-ttu-id="18dd6-138">Especifica quais fontes são incluídas nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="18dd6-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="18dd6-139">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="18dd6-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="18dd6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="18dd6-140">Response</span></span>

<span data-ttu-id="18dd6-141">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [username](../resources/usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18dd6-141">If successful, this method returns a `201 Created` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18dd6-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="18dd6-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18dd6-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18dd6-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="18dd6-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="18dd6-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="18dd6-145">C#</span><span class="sxs-lookup"><span data-stu-id="18dd6-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18dd6-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18dd6-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18dd6-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18dd6-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18dd6-148">Java</span><span class="sxs-lookup"><span data-stu-id="18dd6-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18dd6-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="18dd6-149">Response</span></span>

<span data-ttu-id="18dd6-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="18dd6-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSource"
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
