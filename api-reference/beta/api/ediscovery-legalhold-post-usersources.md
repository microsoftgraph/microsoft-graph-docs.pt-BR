---
title: Criar usuário legalHoldSource
description: Crie um novo objeto legalHold userSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 266ea3603050f34ad77003b9052189abba56baaa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772973"
---
# <a name="create-legalhold-usersource"></a><span data-ttu-id="04eee-103">Criar usuário legalHoldSource</span><span class="sxs-lookup"><span data-stu-id="04eee-103">Create legalHold userSource</span></span>

<span data-ttu-id="04eee-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="04eee-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04eee-105">Adiciona um userSource a um objeto legalHold.</span><span class="sxs-lookup"><span data-stu-id="04eee-105">Adds a userSource to a legalHold object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04eee-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="04eee-106">Permissions</span></span>

<span data-ttu-id="04eee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04eee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04eee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04eee-109">Permission type</span></span>|<span data-ttu-id="04eee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04eee-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04eee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04eee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04eee-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04eee-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="04eee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04eee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04eee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04eee-114">Not supported.</span></span>|
|<span data-ttu-id="04eee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04eee-115">Application</span></span>|<span data-ttu-id="04eee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04eee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04eee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04eee-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="04eee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04eee-118">Request headers</span></span>

|<span data-ttu-id="04eee-119">Nome</span><span class="sxs-lookup"><span data-stu-id="04eee-119">Name</span></span>|<span data-ttu-id="04eee-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="04eee-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="04eee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="04eee-121">Authorization</span></span>|<span data-ttu-id="04eee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04eee-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="04eee-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04eee-124">Content-Type</span></span>|<span data-ttu-id="04eee-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04eee-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04eee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04eee-127">Request body</span></span>

<span data-ttu-id="04eee-128">No corpo da solicitação, fornece uma representação JSON do [objeto userSource.](../resources/ediscovery-usersource.md)</span><span class="sxs-lookup"><span data-stu-id="04eee-128">In the request body, supply a JSON representation of the [userSource](../resources/ediscovery-usersource.md) object.</span></span>

<span data-ttu-id="04eee-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userSource](../resources/ediscovery-usersource.md).</span><span class="sxs-lookup"><span data-stu-id="04eee-129">The following table shows the properties that are required when you create the [userSource](../resources/ediscovery-usersource.md).</span></span>

|<span data-ttu-id="04eee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04eee-130">Property</span></span>|<span data-ttu-id="04eee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="04eee-131">Type</span></span>|<span data-ttu-id="04eee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="04eee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04eee-133">email</span><span class="sxs-lookup"><span data-stu-id="04eee-133">email</span></span>|<span data-ttu-id="04eee-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04eee-134">String</span></span>|<span data-ttu-id="04eee-135">Endereço SMTP do usuário.</span><span class="sxs-lookup"><span data-stu-id="04eee-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="04eee-136">includedSources</span><span class="sxs-lookup"><span data-stu-id="04eee-136">includedSources</span></span>|<span data-ttu-id="04eee-137">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="04eee-137">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="04eee-138">Especifica quais fontes estão incluídas neste grupo.</span><span class="sxs-lookup"><span data-stu-id="04eee-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="04eee-139">Esse valor deve `mailbox` ser , não há suporte para `site` legalHolds no momento.</span><span class="sxs-lookup"><span data-stu-id="04eee-139">This value must be `mailbox`, `site` is not supported for legalHolds at this time.</span></span>|

## <a name="response"></a><span data-ttu-id="04eee-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="04eee-140">Response</span></span>

<span data-ttu-id="04eee-141">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04eee-141">If successful, this method returns a `201 Created` response code and a [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04eee-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="04eee-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04eee-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04eee-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="04eee-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="04eee-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_usersource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources
Content-Type: application/json
Content-length: 208

{
  "email": "adelev@contoso.com",
  "includedSources": "mailbox"
}
```
# <a name="c"></a>[<span data-ttu-id="04eee-145">C#</span><span class="sxs-lookup"><span data-stu-id="04eee-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-usersource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04eee-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04eee-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-usersource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04eee-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04eee-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-usersource-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04eee-148">Java</span><span class="sxs-lookup"><span data-stu-id="04eee-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-usersource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="04eee-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="04eee-149">Response</span></span>

<span data-ttu-id="04eee-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="04eee-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalholds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-12-28T20:08:57.857Z",
            "id": "2192ca40-8ea2-410e-ba3b-ec8ae873be6b",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "EDiscovery admin"
                }
            }
        }
    ]
}
```
