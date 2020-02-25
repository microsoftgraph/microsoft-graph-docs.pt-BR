---
title: 'usuário: translateExchangeIds'
description: Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bad55dd3dc6904f1c329c5a41d54c001162801de
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268347"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="a49e5-103">usuário: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="a49e5-103">user: translateExchangeIds</span></span>

<span data-ttu-id="a49e5-104">Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.</span><span class="sxs-lookup"><span data-stu-id="a49e5-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="a49e5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a49e5-105">Permissions</span></span>

<span data-ttu-id="a49e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a49e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a49e5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a49e5-108">Permission type</span></span> | <span data-ttu-id="a49e5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a49e5-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="a49e5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a49e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a49e5-111">User. ReadBasic. All, User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a49e5-111">User.ReadBasic.All, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="a49e5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a49e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a49e5-113">User. ReadBasic. All, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a49e5-113">User.ReadBasic.All, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="a49e5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a49e5-114">Application</span></span> | <span data-ttu-id="a49e5-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a49e5-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a49e5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a49e5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="a49e5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a49e5-117">Request headers</span></span>

| <span data-ttu-id="a49e5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a49e5-118">Name</span></span> | <span data-ttu-id="a49e5-119">Valor</span><span class="sxs-lookup"><span data-stu-id="a49e5-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="a49e5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a49e5-120">Authorization</span></span> | <span data-ttu-id="a49e5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a49e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a49e5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a49e5-123">Request body</span></span>

| <span data-ttu-id="a49e5-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a49e5-124">Parameter</span></span> | <span data-ttu-id="a49e5-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a49e5-125">Type</span></span> | <span data-ttu-id="a49e5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a49e5-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="a49e5-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="a49e5-127">inputIds</span></span> | <span data-ttu-id="a49e5-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a49e5-128">String collection</span></span> | <span data-ttu-id="a49e5-129">Uma coleção de identificadores a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="a49e5-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="a49e5-130">Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a49e5-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="a49e5-131">O tamanho máximo dessa coleção é de 1000 cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="a49e5-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="a49e5-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="a49e5-132">sourceIdType</span></span> | <span data-ttu-id="a49e5-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="a49e5-133">exchangeIdFormat</span></span> | <span data-ttu-id="a49e5-134">O tipo de ID dos identificadores no `InputIds` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="a49e5-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="a49e5-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="a49e5-135">targetIdType</span></span> | <span data-ttu-id="a49e5-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="a49e5-136">exchangeIdFormat</span></span> | <span data-ttu-id="a49e5-137">O tipo de ID solicitado a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="a49e5-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="a49e5-138">valores de exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="a49e5-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="a49e5-139">Valores</span><span class="sxs-lookup"><span data-stu-id="a49e5-139">Values</span></span> | <span data-ttu-id="a49e5-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="a49e5-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="a49e5-141">entryId</span><span class="sxs-lookup"><span data-stu-id="a49e5-141">entryId</span></span> | <span data-ttu-id="a49e5-142">O formato de ID de entrada binária usado por clientes MAPI.</span><span class="sxs-lookup"><span data-stu-id="a49e5-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="a49e5-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="a49e5-143">ewsId</span></span> | <span data-ttu-id="a49e5-144">O formato de ID usado pelos clientes dos serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a49e5-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="a49e5-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="a49e5-145">immutableEntryId</span></span> | <span data-ttu-id="a49e5-146">O formato de ID imutável binário compatível com MAPI.</span><span class="sxs-lookup"><span data-stu-id="a49e5-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="a49e5-147">restid</span><span class="sxs-lookup"><span data-stu-id="a49e5-147">restId</span></span> | <span data-ttu-id="a49e5-148">O formato de ID padrão usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a49e5-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="a49e5-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="a49e5-149">restImmutableEntryId</span></span> | <span data-ttu-id="a49e5-150">O formato de ID imutável usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a49e5-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="a49e5-151">Os formatos binários`entryId` ( `immutableEntryId`e) são codificados por URL com base em base64.</span><span class="sxs-lookup"><span data-stu-id="a49e5-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="a49e5-152">A segurança de URL é implementada modificando a codificação Base64 dos dados binários da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="a49e5-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="a49e5-153">Substituir `+` por`-`</span><span class="sxs-lookup"><span data-stu-id="a49e5-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="a49e5-154">Substituir `/` por`_`</span><span class="sxs-lookup"><span data-stu-id="a49e5-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="a49e5-155">Remover os caracteres de preenchimento à direita`=`()</span><span class="sxs-lookup"><span data-stu-id="a49e5-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="a49e5-156">Adicione um inteiro ao final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam no original (`0`, `1`, ou) `2`</span><span class="sxs-lookup"><span data-stu-id="a49e5-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="a49e5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="a49e5-157">Response</span></span>

<span data-ttu-id="a49e5-158">Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [convertIdResult](../resources/convertidresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a49e5-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a49e5-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a49e5-159">Example</span></span>

<span data-ttu-id="a49e5-160">O exemplo a seguir mostra como converter vários identificadores do formato de API REST normal (`restId`) para o formato imutável (`restImmutableEntryId`) do REST.</span><span class="sxs-lookup"><span data-stu-id="a49e5-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="a49e5-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a49e5-161">Request</span></span>

<span data-ttu-id="a49e5-162">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="a49e5-162">Here is the example request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a49e5-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="a49e5-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_translateexchangeids"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/translateExchangeIds
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
# <a name="c"></a>[<span data-ttu-id="a49e5-164">C#</span><span class="sxs-lookup"><span data-stu-id="a49e5-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-translateexchangeids-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a49e5-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a49e5-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-translateexchangeids-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a49e5-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a49e5-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-translateexchangeids-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a49e5-167">Java</span><span class="sxs-lookup"><span data-stu-id="a49e5-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-translateexchangeids-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a49e5-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="a49e5-168">Response</span></span>

<span data-ttu-id="a49e5-169">Veja a seguir o exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="a49e5-169">Here is the example response</span></span>
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
