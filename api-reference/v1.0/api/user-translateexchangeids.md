---
title: 'usuário: translateExchangeIds'
description: Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6c3d3401f898b0b086503723ff6de8ff56bc2275
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036414"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="95f4f-103">usuário: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="95f4f-103">user: translateExchangeIds</span></span>

<span data-ttu-id="95f4f-104">Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.</span><span class="sxs-lookup"><span data-stu-id="95f4f-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="95f4f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="95f4f-105">Permissions</span></span>

<span data-ttu-id="95f4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95f4f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95f4f-108">Permission type</span></span> | <span data-ttu-id="95f4f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="95f4f-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="95f4f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95f4f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="95f4f-111">User. ReadBasic, User. Read, User. ReadWrite, User. ReadBasic. All, User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="95f4f-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="95f4f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95f4f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95f4f-113">User. ReadBasic, User. Read, User. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95f4f-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="95f4f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95f4f-114">Application</span></span> | <span data-ttu-id="95f4f-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95f4f-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95f4f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95f4f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="95f4f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95f4f-117">Request headers</span></span>

| <span data-ttu-id="95f4f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="95f4f-118">Name</span></span> | <span data-ttu-id="95f4f-119">Valor</span><span class="sxs-lookup"><span data-stu-id="95f4f-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="95f4f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="95f4f-120">Authorization</span></span> | <span data-ttu-id="95f4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95f4f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95f4f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95f4f-123">Request body</span></span>

| <span data-ttu-id="95f4f-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="95f4f-124">Parameter</span></span> | <span data-ttu-id="95f4f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="95f4f-125">Type</span></span> | <span data-ttu-id="95f4f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="95f4f-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="95f4f-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="95f4f-127">inputIds</span></span> | <span data-ttu-id="95f4f-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="95f4f-128">String collection</span></span> | <span data-ttu-id="95f4f-129">Uma coleção de identificadores a serem convertidos.</span><span class="sxs-lookup"><span data-stu-id="95f4f-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="95f4f-130">Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="95f4f-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="95f4f-131">O tamanho máximo dessa coleção é de 1000 cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="95f4f-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="95f4f-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="95f4f-132">sourceIdType</span></span> | <span data-ttu-id="95f4f-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="95f4f-133">exchangeIdFormat</span></span> | <span data-ttu-id="95f4f-134">O tipo de ID dos identificadores no `InputIds` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="95f4f-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="95f4f-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="95f4f-135">targetIdType</span></span> | <span data-ttu-id="95f4f-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="95f4f-136">exchangeIdFormat</span></span> | <span data-ttu-id="95f4f-137">O tipo de ID solicitado a ser convertido.</span><span class="sxs-lookup"><span data-stu-id="95f4f-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="95f4f-138">valores de exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="95f4f-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="95f4f-139">Valores</span><span class="sxs-lookup"><span data-stu-id="95f4f-139">Values</span></span> | <span data-ttu-id="95f4f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="95f4f-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="95f4f-141">entryId</span><span class="sxs-lookup"><span data-stu-id="95f4f-141">entryId</span></span> | <span data-ttu-id="95f4f-142">O formato de ID de entrada binária usado por clientes MAPI.</span><span class="sxs-lookup"><span data-stu-id="95f4f-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="95f4f-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="95f4f-143">ewsId</span></span> | <span data-ttu-id="95f4f-144">O formato de ID usado pelos clientes dos serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="95f4f-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="95f4f-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="95f4f-145">immutableEntryId</span></span> | <span data-ttu-id="95f4f-146">O formato de ID imutável binário compatível com MAPI.</span><span class="sxs-lookup"><span data-stu-id="95f4f-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="95f4f-147">restid</span><span class="sxs-lookup"><span data-stu-id="95f4f-147">restId</span></span> | <span data-ttu-id="95f4f-148">O formato de ID padrão usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="95f4f-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="95f4f-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="95f4f-149">restImmutableEntryId</span></span> | <span data-ttu-id="95f4f-150">O formato de ID imutável usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="95f4f-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="95f4f-151">Os formatos binários`entryId` ( `immutableEntryId`e) são codificados por URL com base em base64.</span><span class="sxs-lookup"><span data-stu-id="95f4f-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="95f4f-152">A segurança de URL é implementada modificando a codificação Base64 dos dados binários da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="95f4f-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="95f4f-153">Substituir `+` por`-`</span><span class="sxs-lookup"><span data-stu-id="95f4f-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="95f4f-154">Substituir `/` por`_`</span><span class="sxs-lookup"><span data-stu-id="95f4f-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="95f4f-155">Remover os caracteres de preenchimento à direita`=`()</span><span class="sxs-lookup"><span data-stu-id="95f4f-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="95f4f-156">Adicione um inteiro ao final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam no original (`0`, `1`, ou) `2`</span><span class="sxs-lookup"><span data-stu-id="95f4f-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="95f4f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="95f4f-157">Response</span></span>

<span data-ttu-id="95f4f-158">Se bem-sucedido, este método retorna `200 OK` um código de resposta e uma coleção [convertIdResult](../resources/convertidresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95f4f-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95f4f-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95f4f-159">Example</span></span>

<span data-ttu-id="95f4f-160">O exemplo a seguir mostra como converter vários identificadores do formato de API REST normal (`restId`) para o formato imutável (`restImmutableEntryId`) do REST.</span><span class="sxs-lookup"><span data-stu-id="95f4f-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="95f4f-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95f4f-161">Request</span></span>

<span data-ttu-id="95f4f-162">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="95f4f-162">Here is the example request.</span></span>

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

### <a name="response"></a><span data-ttu-id="95f4f-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="95f4f-163">Response</span></span>

<span data-ttu-id="95f4f-164">Veja a seguir o exemplo de resposta</span><span class="sxs-lookup"><span data-stu-id="95f4f-164">Here is the example response</span></span>
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
