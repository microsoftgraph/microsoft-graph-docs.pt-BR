---
title: Listar allowedUsers para impressora
description: Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para a impressora associada.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9cbe7e0c352ab24ccf66283db3c3fd4e1e4dd354
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673738"
---
# <a name="list-allowedusers-for-printer"></a><span data-ttu-id="b34a0-103">Listar allowedUsers para impressora</span><span class="sxs-lookup"><span data-stu-id="b34a0-103">List allowedUsers for printer</span></span>

<span data-ttu-id="b34a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b34a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b34a0-105">Recupere uma lista de usuários que receberam acesso para enviar trabalhos de impressão para a [impressora](../resources/printer.md)associada.</span><span class="sxs-lookup"><span data-stu-id="b34a0-105">Retrieve a list of users who have been granted access to submit print jobs to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b34a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b34a0-106">Permissions</span></span>
<span data-ttu-id="b34a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b34a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b34a0-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b34a0-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="b34a0-110">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="b34a0-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="b34a0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b34a0-111">Permission type</span></span> | <span data-ttu-id="b34a0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b34a0-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b34a0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b34a0-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b34a0-114">Printer. Read. All, Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="b34a0-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="b34a0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b34a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b34a0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b34a0-116">Not Supported.</span></span>|
|<span data-ttu-id="b34a0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b34a0-117">Application</span></span>| <span data-ttu-id="b34a0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b34a0-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b34a0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b34a0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/allowedUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b34a0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b34a0-120">Optional query parameters</span></span>
<span data-ttu-id="b34a0-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b34a0-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b34a0-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b34a0-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b34a0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b34a0-123">Request headers</span></span>
| <span data-ttu-id="b34a0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="b34a0-124">Name</span></span>      |<span data-ttu-id="b34a0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b34a0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b34a0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b34a0-126">Authorization</span></span> | <span data-ttu-id="b34a0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b34a0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b34a0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b34a0-129">Request body</span></span>
<span data-ttu-id="b34a0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b34a0-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b34a0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b34a0-131">Response</span></span>
<span data-ttu-id="b34a0-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [printUserIdentity](../resources/printuseridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b34a0-132">If successful, this method returns a `200 OK` response code and a collection of [printUserIdentity](../resources/printuseridentity.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b34a0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b34a0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b34a0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b34a0-134">Request</span></span>
<span data-ttu-id="b34a0-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b34a0-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b34a0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b34a0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allowedUsers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/allowedUsers
```
# <a name="c"></a>[<span data-ttu-id="b34a0-137">C#</span><span class="sxs-lookup"><span data-stu-id="b34a0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allowedusers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b34a0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b34a0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allowedusers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b34a0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b34a0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allowedusers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b34a0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b34a0-140">Response</span></span>
<span data-ttu-id="b34a0-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b34a0-141">The following is an example of the response.</span></span>
><span data-ttu-id="b34a0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b34a0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUserIdentity",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 286

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.printUserIdentity)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "UserName",
      "userPrincipalName": "username@microsoft.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List allowedUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
