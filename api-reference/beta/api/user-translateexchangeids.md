---
title: 'usuário: translateExchangeIds'
description: Traduza os identificadores de recursos relacionados ao Outlook entre formatos.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b09ae9bf6a1cbf1967a900770b07d8c9750ba21
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571286"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="ec57a-103">usuário: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="ec57a-103">user: translateExchangeIds</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec57a-104">Traduza os identificadores de recursos relacionados ao Outlook entre formatos.</span><span class="sxs-lookup"><span data-stu-id="ec57a-104">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec57a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec57a-105">Permissions</span></span>

<span data-ttu-id="ec57a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec57a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec57a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec57a-108">Permission type</span></span> | <span data-ttu-id="ec57a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec57a-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="ec57a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec57a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec57a-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec57a-111">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="ec57a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec57a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec57a-113">User.ReadBasic, User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec57a-113">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="ec57a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec57a-114">Application</span></span> | <span data-ttu-id="ec57a-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec57a-115">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec57a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec57a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="ec57a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec57a-117">Request headers</span></span>

| <span data-ttu-id="ec57a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ec57a-118">Name</span></span> | <span data-ttu-id="ec57a-119">Valor</span><span class="sxs-lookup"><span data-stu-id="ec57a-119">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="ec57a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec57a-120">Authorization</span></span> | <span data-ttu-id="ec57a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec57a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec57a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec57a-123">Request body</span></span>

| <span data-ttu-id="ec57a-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ec57a-124">Parameter</span></span> | <span data-ttu-id="ec57a-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec57a-125">Type</span></span> | <span data-ttu-id="ec57a-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec57a-126">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="ec57a-127">inputIds</span><span class="sxs-lookup"><span data-stu-id="ec57a-127">inputIds</span></span> | <span data-ttu-id="ec57a-128">Coleção Edm.String</span><span class="sxs-lookup"><span data-stu-id="ec57a-128">Edm.String collection</span></span> | <span data-ttu-id="ec57a-129">Uma coleção de identificadores para converter.</span><span class="sxs-lookup"><span data-stu-id="ec57a-129">A collection of identifiers to convert.</span></span> <span data-ttu-id="ec57a-130">Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ec57a-130">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="ec57a-131">Tamanho máximo dessa coleção é 1000 cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="ec57a-131">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="ec57a-132">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="ec57a-132">sourceIdType</span></span> | <span data-ttu-id="ec57a-133">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="ec57a-133">exchangeIdFormat</span></span> | <span data-ttu-id="ec57a-134">O tipo de identificadores de na ID do `InputIds` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="ec57a-134">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="ec57a-135">targetIdType</span><span class="sxs-lookup"><span data-stu-id="ec57a-135">targetIdType</span></span> | <span data-ttu-id="ec57a-136">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="ec57a-136">exchangeIdFormat</span></span> | <span data-ttu-id="ec57a-137">O tipo de ID solicitado para converter em.</span><span class="sxs-lookup"><span data-stu-id="ec57a-137">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="ec57a-138">valores de exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="ec57a-138">exchangeIdFormat values</span></span>

| <span data-ttu-id="ec57a-139">Valores</span><span class="sxs-lookup"><span data-stu-id="ec57a-139">Values</span></span> | <span data-ttu-id="ec57a-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec57a-140">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="ec57a-141">entryId</span><span class="sxs-lookup"><span data-stu-id="ec57a-141">entryId</span></span> | <span data-ttu-id="ec57a-142">O formato de ID de entrada binário usado pelos clientes MAPI.</span><span class="sxs-lookup"><span data-stu-id="ec57a-142">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="ec57a-143">ewsId</span><span class="sxs-lookup"><span data-stu-id="ec57a-143">ewsId</span></span> | <span data-ttu-id="ec57a-144">O formato de ID usado pelos clientes de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec57a-144">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="ec57a-145">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="ec57a-145">immutableEntryId</span></span> | <span data-ttu-id="ec57a-146">O compatível com MAPI imutável ID formato binário.</span><span class="sxs-lookup"><span data-stu-id="ec57a-146">The binary MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="ec57a-147">restId</span><span class="sxs-lookup"><span data-stu-id="ec57a-147">restId</span></span> | <span data-ttu-id="ec57a-148">O formato de ID padrão usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ec57a-148">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="ec57a-149">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="ec57a-149">restImmutableEntryId</span></span> | <span data-ttu-id="ec57a-150">O formato de ID imutável usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ec57a-150">The immutable ID format used by Microsoft Graph.</span></span> |

<span data-ttu-id="ec57a-151">Formatos binários (`entryId` e `immutableEntryId`) são URL-safe codificação base64.</span><span class="sxs-lookup"><span data-stu-id="ec57a-151">The binary formats (`entryId` and `immutableEntryId`) are URL-safe base64 encoded.</span></span> <span data-ttu-id="ec57a-152">URL-safeness é implementado, modificando a codificação base64 dos dados binários da seguinte maneira:</span><span class="sxs-lookup"><span data-stu-id="ec57a-152">URL-safeness is implemented by modifying the base64 encoding of the binary data in the following way:</span></span>

- <span data-ttu-id="ec57a-153">Substituir `+` com`-`</span><span class="sxs-lookup"><span data-stu-id="ec57a-153">Replace `+` with `-`</span></span>
- <span data-ttu-id="ec57a-154">Substituir `/` com`_`</span><span class="sxs-lookup"><span data-stu-id="ec57a-154">Replace `/` with `_`</span></span>
- <span data-ttu-id="ec57a-155">Remova os caracteres de preenchimento à direita (`=`)</span><span class="sxs-lookup"><span data-stu-id="ec57a-155">Remove any trailing padding characters (`=`)</span></span>
- <span data-ttu-id="ec57a-156">Adicionar um número inteiro até o final da cadeia de caracteres indicando quantos caracteres de preenchimento estavam em original (`0`, `1`, ou `2`)</span><span class="sxs-lookup"><span data-stu-id="ec57a-156">Add an integer to the end of the string indicating how many padding characters were in the original (`0`, `1`, or `2`)</span></span>

## <a name="response"></a><span data-ttu-id="ec57a-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec57a-157">Response</span></span>

<span data-ttu-id="ec57a-158">Se tiver êxito, este método retornará `200 OK` código de resposta e um conjunto de [convertIdResult](../resources/convertidresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec57a-158">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/convertidresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec57a-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec57a-159">Example</span></span>

<span data-ttu-id="ec57a-160">O exemplo a seguir mostra como converter vários identificadores do formato de API REST do normal (`restId`) para o formato de imutável REST (`restImmutableEntryId`).</span><span class="sxs-lookup"><span data-stu-id="ec57a-160">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

### <a name="request"></a><span data-ttu-id="ec57a-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec57a-161">Request</span></span>

<span data-ttu-id="ec57a-162">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="ec57a-162">Here is the example request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec57a-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec57a-163">Response</span></span>

<span data-ttu-id="ec57a-164">Aqui está a resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="ec57a-164">Here is the example response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-translateexchangeids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
