---
title: 'usuário: translateExchangeIds'
description: Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b62027af1f21df9118fe278a8ad1b04f6796fe5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269444"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="9f4a8-103">usuário: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="9f4a8-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f4a8-104">Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f4a8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9f4a8-105">Permissions</span></span>

<span data-ttu-id="9f4a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f4a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9f4a8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f4a8-108">Permission type</span></span> | <span data-ttu-id="9f4a8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f4a8-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="9f4a8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f4a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9f4a8-111">User. ReadBasic, User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9f4a8-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="9f4a8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f4a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f4a8-113">User. ReadBasic, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f4a8-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="9f4a8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f4a8-114">Application</span></span> | <span data-ttu-id="9f4a8-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f4a8-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f4a8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f4a8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="9f4a8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f4a8-117">Request headers</span></span>

| <span data-ttu-id="9f4a8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9f4a8-118">Name</span></span> | <span data-ttu-id="9f4a8-119">Valor</span><span class="sxs-lookup"><span data-stu-id="9f4a8-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="9f4a8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f4a8-120">Authorization</span></span> | <span data-ttu-id="9f4a8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f4a8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f4a8-123">Request body</span></span>

| <span data-ttu-id="9f4a8-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9f4a8-124">Parameter</span></span> | <span data-ttu-id="9f4a8-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f4a8-125">Type</span></span> | <span data-ttu-id="9f4a8-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f4a8-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="9f4a8-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="9f4a8-127">inputIds</span></span> | <span data-ttu-id="9f4a8-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f4a8-128">String collection</span></span> | <span data-ttu-id="9f4a8-129">Uma coleção de identificadores a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="9f4a8-130">Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="9f4a8-131">O tamanho máximo dessa coleção é de 1000 cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="9f4a8-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="9f4a8-132">sourceIdType</span></span> | <span data-ttu-id="9f4a8-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="9f4a8-133">exchangeIdFormat</span></span> | <span data-ttu-id="9f4a8-134">O tipo de ID dos identificadores no `InputIds` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="9f4a8-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="9f4a8-135">targetIdType</span></span> | <span data-ttu-id="9f4a8-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="9f4a8-136">exchangeIdFormat</span></span> | <span data-ttu-id="9f4a8-137">O tipo de ID solicitado a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="9f4a8-138">valores de exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="9f4a8-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="9f4a8-139">Valores</span><span class="sxs-lookup"><span data-stu-id="9f4a8-139">Values</span></span> | <span data-ttu-id="9f4a8-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f4a8-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="9f4a8-141">entryId</span><span class="sxs-lookup"><span data-stu-id="9f4a8-141">entryId</span></span> | <span data-ttu-id="9f4a8-142">O formato de ID de entrada binária usado por clientes MAPI.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="9f4a8-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="9f4a8-143">ewsId</span></span> | <span data-ttu-id="9f4a8-144">O formato de ID usado pelos clientes dos serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="9f4a8-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="9f4a8-145">immutableEntryId</span></span> | <span data-ttu-id="9f4a8-146">O formato de ID imutável binário compatível com MAPI.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="9f4a8-147">restid</span><span class="sxs-lookup"><span data-stu-id="9f4a8-147">restId</span></span> | <span data-ttu-id="9f4a8-148">O formato de ID padrão usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="9f4a8-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="9f4a8-149">restImmutableEntryId</span></span> | <span data-ttu-id="9f4a8-150">O formato de ID imutável usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="9f4a8-151">Os formatos binários`entryId` ( `immutableEntryId`e) são codificados por URL com base em base64.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="9f4a8-152">A segurança de URL é implementada modificando a codificação Base64 dos dados binários da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="9f4a8-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="9f4a8-153">Substituir `+` por`-`</span><span class="sxs-lookup"><span data-stu-id="9f4a8-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="9f4a8-154">Substituir `/` por`_`</span><span class="sxs-lookup"><span data-stu-id="9f4a8-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="9f4a8-155">Remover os caracteres de preenchimento à direita`=`()</span><span class="sxs-lookup"><span data-stu-id="9f4a8-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="9f4a8-156">Adicione um inteiro ao final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam no original (`0`, `1`, ou) `2`</span><span class="sxs-lookup"><span data-stu-id="9f4a8-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="9f4a8-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f4a8-157">Response</span></span>

<span data-ttu-id="9f4a8-158">Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [convertIdResult](../resources/convertidresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f4a8-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f4a8-159">Example</span></span>

<span data-ttu-id="9f4a8-160">O exemplo a seguir mostra como converter vários identificadores do formato de API REST normal (`restId`) para o formato imutável (`restImmutableEntryId`) do REST.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="9f4a8-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f4a8-161">Request</span></span>

<span data-ttu-id="9f4a8-162">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="9f4a8-162">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f4a8-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f4a8-163">Response</span></span>

<span data-ttu-id="9f4a8-164">Veja a seguir o exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="9f4a8-164">Here is the example response</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9f4a8-165">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="9f4a8-165">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9f4a8-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="9f4a8-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="9f4a8-167">C#</span><span class="sxs-lookup"><span data-stu-id="9f4a8-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9f4a8-168">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9f4a8-168">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_translateexchangeids-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
