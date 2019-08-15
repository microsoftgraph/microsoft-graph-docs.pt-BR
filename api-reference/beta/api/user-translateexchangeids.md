---
title: 'usuário: translateExchangeIds'
description: Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6eb044c42ce01c13e45e7088fa3eb6f96fb4820a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421803"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="112b6-103">usuário: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="112b6-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="112b6-104">Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.</span><span class="sxs-lookup"><span data-stu-id="112b6-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="112b6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="112b6-105">Permissions</span></span>

<span data-ttu-id="112b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="112b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="112b6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="112b6-108">Permission type</span></span> | <span data-ttu-id="112b6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="112b6-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="112b6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="112b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="112b6-111">User. ReadBasic, User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="112b6-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="112b6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="112b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="112b6-113">User. ReadBasic, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="112b6-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="112b6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="112b6-114">Application</span></span> | <span data-ttu-id="112b6-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="112b6-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="112b6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="112b6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="112b6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="112b6-117">Request headers</span></span>

| <span data-ttu-id="112b6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="112b6-118">Name</span></span> | <span data-ttu-id="112b6-119">Valor</span><span class="sxs-lookup"><span data-stu-id="112b6-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="112b6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="112b6-120">Authorization</span></span> | <span data-ttu-id="112b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="112b6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="112b6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="112b6-123">Request body</span></span>

| <span data-ttu-id="112b6-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="112b6-124">Parameter</span></span> | <span data-ttu-id="112b6-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="112b6-125">Type</span></span> | <span data-ttu-id="112b6-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="112b6-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="112b6-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="112b6-127">inputIds</span></span> | <span data-ttu-id="112b6-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="112b6-128">String collection</span></span> | <span data-ttu-id="112b6-129">Uma coleção de identificadores a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="112b6-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="112b6-130">Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="112b6-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="112b6-131">O tamanho máximo dessa coleção é de 1000 cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="112b6-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="112b6-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="112b6-132">sourceIdType</span></span> | <span data-ttu-id="112b6-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="112b6-133">exchangeIdFormat</span></span> | <span data-ttu-id="112b6-134">O tipo de ID dos identificadores no `InputIds` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="112b6-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="112b6-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="112b6-135">targetIdType</span></span> | <span data-ttu-id="112b6-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="112b6-136">exchangeIdFormat</span></span> | <span data-ttu-id="112b6-137">O tipo de ID solicitado a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="112b6-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="112b6-138">valores de exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="112b6-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="112b6-139">Valores</span><span class="sxs-lookup"><span data-stu-id="112b6-139">Values</span></span> | <span data-ttu-id="112b6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="112b6-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="112b6-141">entryId</span><span class="sxs-lookup"><span data-stu-id="112b6-141">entryId</span></span> | <span data-ttu-id="112b6-142">O formato de ID de entrada binária usado por clientes MAPI.</span><span class="sxs-lookup"><span data-stu-id="112b6-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="112b6-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="112b6-143">ewsId</span></span> | <span data-ttu-id="112b6-144">O formato de ID usado pelos clientes dos serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="112b6-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="112b6-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="112b6-145">immutableEntryId</span></span> | <span data-ttu-id="112b6-146">O formato de ID imutável binário compatível com MAPI.</span><span class="sxs-lookup"><span data-stu-id="112b6-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="112b6-147">restid</span><span class="sxs-lookup"><span data-stu-id="112b6-147">restId</span></span> | <span data-ttu-id="112b6-148">O formato de ID padrão usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="112b6-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="112b6-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="112b6-149">restImmutableEntryId</span></span> | <span data-ttu-id="112b6-150">O formato de ID imutável usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="112b6-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="112b6-151">Os formatos binários`entryId` ( `immutableEntryId`e) são codificados por URL com base em base64.</span><span class="sxs-lookup"><span data-stu-id="112b6-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="112b6-152">A segurança de URL é implementada modificando a codificação Base64 dos dados binários da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="112b6-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="112b6-153">Substituir `+` por`-`</span><span class="sxs-lookup"><span data-stu-id="112b6-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="112b6-154">Substituir `/` por`_`</span><span class="sxs-lookup"><span data-stu-id="112b6-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="112b6-155">Remover os caracteres de preenchimento à direita`=`()</span><span class="sxs-lookup"><span data-stu-id="112b6-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="112b6-156">Adicione um inteiro ao final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam no original (`0`, `1`, ou) `2`</span><span class="sxs-lookup"><span data-stu-id="112b6-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="112b6-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="112b6-157">Response</span></span>

<span data-ttu-id="112b6-158">Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [convertIdResult](../resources/convertidresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="112b6-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="112b6-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="112b6-159">Example</span></span>

<span data-ttu-id="112b6-160">O exemplo a seguir mostra como converter vários identificadores do formato de API REST normal (`restId`) para o formato imutável (`restImmutableEntryId`) do REST.</span><span class="sxs-lookup"><span data-stu-id="112b6-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="112b6-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="112b6-161">Request</span></span>

<span data-ttu-id="112b6-162">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="112b6-162">Here is the example request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="112b6-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="112b6-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/beta/me/translateExchangeIds
Content-Type: application/json

{
  "inputIds" : [
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
  ],
  "sourceIdType": "restId",
  "targetIdType": "restImmutableEntryId"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="112b6-164">C#</span><span class="sxs-lookup"><span data-stu-id="112b6-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="112b6-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="112b6-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="112b6-166">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="112b6-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="112b6-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="112b6-167">Response</span></span>

<span data-ttu-id="112b6-168">Veja a seguir o exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="112b6-168">Here is the example response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/testexchangebeta/$metadata#Collection(microsoft.graph.convertIdResult)",
  "value": [
    {
      "sourceId": "{rest-formatted-id-1}",
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2}",
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
