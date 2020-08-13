---
title: 'usuário: translateExchangeIds'
description: Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ae26f5b5a5a109145daa132837890943a98c8c0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451622"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="d15aa-103">usuário: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="d15aa-103">user: translateExchangeIds</span></span>

<span data-ttu-id="d15aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d15aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d15aa-105">Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.</span><span class="sxs-lookup"><span data-stu-id="d15aa-105">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="d15aa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d15aa-106">Permissions</span></span>

<span data-ttu-id="d15aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d15aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d15aa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d15aa-109">Permission type</span></span> | <span data-ttu-id="d15aa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d15aa-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="d15aa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d15aa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d15aa-112">User. ReadBasic. All, User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d15aa-112">User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="d15aa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d15aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d15aa-114">User. ReadBasic. All, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d15aa-114">User.ReadBasic.All, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="d15aa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d15aa-115">Application</span></span> | <span data-ttu-id="d15aa-116">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d15aa-116">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d15aa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d15aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="d15aa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d15aa-118">Request headers</span></span>

| <span data-ttu-id="d15aa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d15aa-119">Name</span></span> | <span data-ttu-id="d15aa-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d15aa-120">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="d15aa-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d15aa-121">Authorization</span></span> | <span data-ttu-id="d15aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d15aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d15aa-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d15aa-124">Request body</span></span>

| <span data-ttu-id="d15aa-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d15aa-125">Parameter</span></span> | <span data-ttu-id="d15aa-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d15aa-126">Type</span></span> | <span data-ttu-id="d15aa-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d15aa-127">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="d15aa-128">inputIds</span><span class="sxs-lookup"><span data-stu-id="d15aa-128">inputIds</span></span> | <span data-ttu-id="d15aa-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d15aa-129">String collection</span></span> | <span data-ttu-id="d15aa-130">Uma coleção de identificadores a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="d15aa-130">A collection of identifiers to convert.</span></span> <span data-ttu-id="d15aa-131">Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d15aa-131">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="d15aa-132">O tamanho máximo dessa coleção é de 1000 cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="d15aa-132">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="d15aa-133">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="d15aa-133">sourceIdType</span></span> | <span data-ttu-id="d15aa-134">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="d15aa-134">exchangeIdFormat</span></span> | <span data-ttu-id="d15aa-135">O tipo de ID dos identificadores no `InputIds` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="d15aa-135">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="d15aa-136">targetIdType</span><span class="sxs-lookup"><span data-stu-id="d15aa-136">targetIdType</span></span> | <span data-ttu-id="d15aa-137">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="d15aa-137">exchangeIdFormat</span></span> | <span data-ttu-id="d15aa-138">O tipo de ID solicitado a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="d15aa-138">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="d15aa-139">valores de exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="d15aa-139">exchangeIdFormat values</span></span>

| <span data-ttu-id="d15aa-140">Valores</span><span class="sxs-lookup"><span data-stu-id="d15aa-140">Values</span></span> | <span data-ttu-id="d15aa-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="d15aa-141">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="d15aa-142">entryId</span><span class="sxs-lookup"><span data-stu-id="d15aa-142">entryId</span></span> | <span data-ttu-id="d15aa-143">O formato de ID de entrada binária usado por clientes MAPI.</span><span class="sxs-lookup"><span data-stu-id="d15aa-143">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="d15aa-144">ewsId</span><span class="sxs-lookup"><span data-stu-id="d15aa-144">ewsId</span></span> | <span data-ttu-id="d15aa-145">O formato de ID usado pelos clientes dos serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d15aa-145">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="d15aa-146">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="d15aa-146">immutableEntryId</span></span> | <span data-ttu-id="d15aa-147">O formato de ID imutável binário compatível com MAPI.</span><span class="sxs-lookup"><span data-stu-id="d15aa-147">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="d15aa-148">restid</span><span class="sxs-lookup"><span data-stu-id="d15aa-148">restId</span></span> | <span data-ttu-id="d15aa-149">O formato de ID padrão usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d15aa-149">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="d15aa-150">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="d15aa-150">restImmutableEntryId</span></span> | <span data-ttu-id="d15aa-151">O formato de ID imutável usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d15aa-151">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="d15aa-152">Os formatos binários ( `entryId` e `immutableEntryId` ) são codificados por URL com base em base64.</span><span class="sxs-lookup"><span data-stu-id="d15aa-152">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="d15aa-153">A segurança de URL é implementada modificando a codificação Base64 dos dados binários da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="d15aa-153">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="d15aa-154">Substituir `+` por`-`</span><span class="sxs-lookup"><span data-stu-id="d15aa-154">Replace `+` with `-`</span></span>
- <span data-ttu-id="d15aa-155">Substituir `/` por`_`</span><span class="sxs-lookup"><span data-stu-id="d15aa-155">Replace `/` with `_`</span></span>
- <span data-ttu-id="d15aa-156">Remover os caracteres de preenchimento à direita ( `=` )</span><span class="sxs-lookup"><span data-stu-id="d15aa-156">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="d15aa-157">Adicione um inteiro ao final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam no original ( `0` , `1` , ou `2` )</span><span class="sxs-lookup"><span data-stu-id="d15aa-157">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="d15aa-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="d15aa-158">Response</span></span>

<span data-ttu-id="d15aa-159">Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [convertIdResult](../resources/convertidresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d15aa-159">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d15aa-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d15aa-160">Example</span></span>

<span data-ttu-id="d15aa-161">O exemplo a seguir mostra como converter vários identificadores do formato de API REST normal ( `restId` ) para o formato imutável () do REST `restImmutableEntryId` .</span><span class="sxs-lookup"><span data-stu-id="d15aa-161">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="d15aa-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d15aa-162">Request</span></span>

<span data-ttu-id="d15aa-163">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="d15aa-163">Here is the example request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d15aa-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="d15aa-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d15aa-165">C#</span><span class="sxs-lookup"><span data-stu-id="d15aa-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d15aa-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d15aa-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d15aa-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d15aa-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d15aa-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="d15aa-168">Response</span></span>

<span data-ttu-id="d15aa-169">Veja a seguir o exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="d15aa-169">Here is the example response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.convertIdResult",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
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
