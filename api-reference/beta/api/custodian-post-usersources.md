---
title: Criar userSource
description: Crie um novo objeto userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 0534acf5e440105f3f423ce3d96d98db98d093f0
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872517"
---
# <a name="create-usersource"></a><span data-ttu-id="bec9e-103">Criar userSource</span><span class="sxs-lookup"><span data-stu-id="bec9e-103">Create userSource</span></span>

<span data-ttu-id="bec9e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bec9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bec9e-105">Crie um novo [objeto userSource.](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="bec9e-105">Create a new [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bec9e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bec9e-106">Permissions</span></span>

<span data-ttu-id="bec9e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bec9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bec9e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bec9e-109">Permission type</span></span>|<span data-ttu-id="bec9e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bec9e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bec9e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bec9e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bec9e-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="bec9e-112">User.Read</span></span>|
|<span data-ttu-id="bec9e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bec9e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bec9e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bec9e-114">Not supported.</span></span>|
|<span data-ttu-id="bec9e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bec9e-115">Application</span></span>|<span data-ttu-id="bec9e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bec9e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bec9e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bec9e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="bec9e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bec9e-118">Request headers</span></span>

|<span data-ttu-id="bec9e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bec9e-119">Name</span></span>|<span data-ttu-id="bec9e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bec9e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bec9e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bec9e-121">Authorization</span></span>|<span data-ttu-id="bec9e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bec9e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bec9e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bec9e-124">Content-Type</span></span>|<span data-ttu-id="bec9e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bec9e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bec9e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bec9e-127">Request body</span></span>

<span data-ttu-id="bec9e-128">No corpo da solicitação, fornece uma representação JSON do [objeto userSource.](../resources/usersource.md)</span><span class="sxs-lookup"><span data-stu-id="bec9e-128">In the request body, supply a JSON representation of the [userSource](../resources/usersource.md) object.</span></span>

<span data-ttu-id="bec9e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userSource](../resources/usersource.md).</span><span class="sxs-lookup"><span data-stu-id="bec9e-129">The following table shows the properties that are required when you create the [userSource](../resources/usersource.md).</span></span>

|<span data-ttu-id="bec9e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bec9e-130">Property</span></span>|<span data-ttu-id="bec9e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bec9e-131">Type</span></span>|<span data-ttu-id="bec9e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bec9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bec9e-133">email</span><span class="sxs-lookup"><span data-stu-id="bec9e-133">email</span></span>|<span data-ttu-id="bec9e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bec9e-134">String</span></span>|<span data-ttu-id="bec9e-135">Endereço SMTP do usuário.</span><span class="sxs-lookup"><span data-stu-id="bec9e-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="bec9e-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="bec9e-136">includedSources</span></span>|<span data-ttu-id="bec9e-137">sourceType</span><span class="sxs-lookup"><span data-stu-id="bec9e-137">sourceType</span></span>|<span data-ttu-id="bec9e-138">Especifica quais fontes estão incluídas nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="bec9e-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="bec9e-139">Os valores possíveis são: `mailbox` e `site`.</span><span class="sxs-lookup"><span data-stu-id="bec9e-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="bec9e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bec9e-140">Response</span></span>

<span data-ttu-id="bec9e-141">Se bem-sucedido, este método retorna um código de resposta e um `201 Created` [objeto userSource](../resources/usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bec9e-141">If successful, this method returns a `201 Created` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bec9e-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bec9e-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bec9e-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bec9e-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bec9e-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="bec9e-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bec9e-145">C#</span><span class="sxs-lookup"><span data-stu-id="bec9e-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bec9e-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bec9e-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bec9e-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bec9e-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bec9e-148">Java</span><span class="sxs-lookup"><span data-stu-id="bec9e-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bec9e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="bec9e-149">Response</span></span>

<span data-ttu-id="bec9e-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bec9e-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
