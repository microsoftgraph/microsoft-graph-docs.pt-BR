---
title: 'usuário: translateExchangeIds'
description: Traduza os identificadores de recursos relacionados ao Outlook entre formatos.
ms.openlocfilehash: 0c6e74ad0bb9676f261ed0202757b1e036b09c85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037582"
---
# <a name="user-translateexchangeids"></a><span data-ttu-id="b7092-103">usuário: translateExchangeIds</span><span class="sxs-lookup"><span data-stu-id="b7092-103">user: translateExchangeIds</span></span>

> <span data-ttu-id="b7092-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b7092-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7092-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b7092-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7092-106">Traduza os identificadores de recursos relacionados ao Outlook entre formatos.</span><span class="sxs-lookup"><span data-stu-id="b7092-106">Translate identifiers of Outlook-related resources between formats.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7092-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="b7092-107">Permissions</span></span>

<span data-ttu-id="b7092-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7092-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7092-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7092-110">Permission type</span></span> | <span data-ttu-id="b7092-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7092-111">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
| <span data-ttu-id="b7092-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7092-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b7092-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7092-113">User.ReadBasic, User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="b7092-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7092-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7092-115">User.ReadBasic, User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7092-115">User.ReadBasic, User.Read, User.ReadWrite</span></span> |
| <span data-ttu-id="b7092-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7092-116">Application</span></span> | <span data-ttu-id="b7092-117">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7092-117">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7092-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7092-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/translateExchangeIds
POST /users/{id|userPrincipalName}/translateExchangeIds
```

## <a name="request-headers"></a><span data-ttu-id="b7092-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7092-119">Request headers</span></span>

| <span data-ttu-id="b7092-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b7092-120">Name</span></span> | <span data-ttu-id="b7092-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b7092-121">Value</span></span> |
|:-----|:------|
| <span data-ttu-id="b7092-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7092-122">Authorization</span></span> | <span data-ttu-id="b7092-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7092-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7092-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7092-125">Request body</span></span>

| <span data-ttu-id="b7092-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b7092-126">Parameter</span></span> | <span data-ttu-id="b7092-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7092-127">Type</span></span> | <span data-ttu-id="b7092-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7092-128">Description</span></span> |
|:----------|:-----|:------------|
| <span data-ttu-id="b7092-129">inputIds</span><span class="sxs-lookup"><span data-stu-id="b7092-129">inputIds</span></span> | <span data-ttu-id="b7092-130">Coleção Edm.String</span><span class="sxs-lookup"><span data-stu-id="b7092-130">Edm.String collection</span></span> | <span data-ttu-id="b7092-131">Uma coleção de identificadores para converter.</span><span class="sxs-lookup"><span data-stu-id="b7092-131">A collection of identifiers to convert.</span></span> <span data-ttu-id="b7092-132">Todos os identificadores na coleção devem ter o mesmo tipo de ID de fonte e devem ser para itens na mesma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b7092-132">All identifiers in the collection MUST have the same source ID type, and MUST be for items in the same mailbox.</span></span> <span data-ttu-id="b7092-133">Tamanho máximo dessa coleção é 1000 cadeias de caracteres.</span><span class="sxs-lookup"><span data-stu-id="b7092-133">Maximum size of this collection is 1000 strings.</span></span> |
| <span data-ttu-id="b7092-134">sourceIdType</span><span class="sxs-lookup"><span data-stu-id="b7092-134">sourceIdType</span></span> | <span data-ttu-id="b7092-135">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="b7092-135">exchangeIdFormat</span></span> | <span data-ttu-id="b7092-136">O tipo de identificadores de na ID do `InputIds` parâmetro.</span><span class="sxs-lookup"><span data-stu-id="b7092-136">The ID type of the identifiers in the `InputIds` parameter.</span></span> |
| <span data-ttu-id="b7092-137">targetIdType</span><span class="sxs-lookup"><span data-stu-id="b7092-137">targetIdType</span></span> | <span data-ttu-id="b7092-138">exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="b7092-138">exchangeIdFormat</span></span> | <span data-ttu-id="b7092-139">O tipo de ID solicitado para converter em.</span><span class="sxs-lookup"><span data-stu-id="b7092-139">The requested ID type to convert to.</span></span> |

### <a name="exchangeidformat-values"></a><span data-ttu-id="b7092-140">valores de exchangeIdFormat</span><span class="sxs-lookup"><span data-stu-id="b7092-140">exchangeIdFormat values</span></span>

| <span data-ttu-id="b7092-141">Valores</span><span class="sxs-lookup"><span data-stu-id="b7092-141">Values</span></span> | <span data-ttu-id="b7092-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7092-142">Description</span></span> |
|:-------|:------------|
| <span data-ttu-id="b7092-143">entryId</span><span class="sxs-lookup"><span data-stu-id="b7092-143">entryId</span></span> | <span data-ttu-id="b7092-144">O formato de ID de entrada binário usado pelos clientes MAPI.</span><span class="sxs-lookup"><span data-stu-id="b7092-144">The binary entry ID format used by MAPI clients.</span></span> |
| <span data-ttu-id="b7092-145">ewsId</span><span class="sxs-lookup"><span data-stu-id="b7092-145">ewsId</span></span> | <span data-ttu-id="b7092-146">O formato de ID usado pelos clientes de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7092-146">The ID format used by Exchange Web Services clients.</span></span> |
| <span data-ttu-id="b7092-147">immutableEntryId</span><span class="sxs-lookup"><span data-stu-id="b7092-147">immutableEntryId</span></span> | <span data-ttu-id="b7092-148">O formato de ID imutável compatível com MAPI.</span><span class="sxs-lookup"><span data-stu-id="b7092-148">The MAPI-compatible immutable ID format.</span></span> |
| <span data-ttu-id="b7092-149">restId</span><span class="sxs-lookup"><span data-stu-id="b7092-149">restId</span></span> | <span data-ttu-id="b7092-150">O formato de ID padrão usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b7092-150">The default ID format used by Microsoft Graph.</span></span> |
| <span data-ttu-id="b7092-151">restImmutableEntryId</span><span class="sxs-lookup"><span data-stu-id="b7092-151">restImmutableEntryId</span></span> | <span data-ttu-id="b7092-152">O formato de ID imutável usado pelo Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b7092-152">The immutable ID format used by Microsoft Graph.</span></span> |

## <a name="response"></a><span data-ttu-id="b7092-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7092-153">Response</span></span>

<span data-ttu-id="b7092-154">Se tiver êxito, este método retornará `200 OK` código de resposta e um conjunto de [convertIdResult](../resources/meetingtimesuggestionsresult.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7092-154">If successful, this method returns `200 OK` response code and a [convertIdResult](../resources/meetingtimesuggestionsresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7092-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7092-155">Example</span></span>

<span data-ttu-id="b7092-156">O exemplo a seguir mostra como converter vários identificadores do formato de API REST do normal (`restId`) para o formato de imutável REST (`restImmutableEntryId`).</span><span class="sxs-lookup"><span data-stu-id="b7092-156">The following example shows how to convert multiple identifiers from the normal REST API format (`restId`) to the REST immutable format (`restImmutableEntryId`).</span></span>

##### <a name="request"></a><span data-ttu-id="b7092-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7092-157">Request</span></span>

<span data-ttu-id="b7092-158">Aqui está a solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="b7092-158">Here is the example request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b7092-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7092-159">Response</span></span>

<span data-ttu-id="b7092-160">Aqui está a resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="b7092-160">Here is the example response</span></span>
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
      "sourceId": "{rest-formatted-id-1},
      "targetId": "{rest-immutable-formatted-id-1}"
    },
    {
      "sourceId": "{rest-formatted-id-2},
      "targetId": "{rest-immutable-formatted-id-2}"
    }
  ]
}
```