---
title: Obter printSettings
description: Recupere configurações de todo o locatário para o serviço de impressão universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e60d8ed8c2c0257f718784297bfba358939a1d6b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314955"
---
# <a name="get-printsettings"></a><span data-ttu-id="1ecb9-103">Obter printSettings</span><span class="sxs-lookup"><span data-stu-id="1ecb9-103">Get printSettings</span></span>

<span data-ttu-id="1ecb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ecb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ecb9-105">Recupere configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ecb9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ecb9-106">Permissions</span></span>
<span data-ttu-id="1ecb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ecb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1ecb9-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="1ecb9-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="1ecb9-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="1ecb9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ecb9-111">Permission type</span></span> | <span data-ttu-id="1ecb9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ecb9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="1ecb9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ecb9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="1ecb9-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="1ecb9-114">User.Read</span></span> |
|<span data-ttu-id="1ecb9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ecb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ecb9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-116">Not Supported.</span></span>|
|<span data-ttu-id="1ecb9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ecb9-117">Application</span></span>|<span data-ttu-id="1ecb9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ecb9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ecb9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ecb9-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1ecb9-120">Optional query parameters</span></span>
<span data-ttu-id="1ecb9-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1ecb9-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1ecb9-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ecb9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecb9-123">Request headers</span></span>
| <span data-ttu-id="1ecb9-124">Nome</span><span class="sxs-lookup"><span data-stu-id="1ecb9-124">Name</span></span>      |<span data-ttu-id="1ecb9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ecb9-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ecb9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ecb9-126">Authorization</span></span> | <span data-ttu-id="1ecb9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ecb9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecb9-129">Request body</span></span>
<span data-ttu-id="1ecb9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1ecb9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ecb9-131">Response</span></span>
<span data-ttu-id="1ecb9-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printSettings](../resources/printsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-132">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ecb9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ecb9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ecb9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ecb9-134">Request</span></span>
<span data-ttu-id="1ecb9-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ecb9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ecb9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/settings
```
# <a name="c"></a>[<span data-ttu-id="1ecb9-137">C#</span><span class="sxs-lookup"><span data-stu-id="1ecb9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ecb9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ecb9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ecb9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ecb9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1ecb9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ecb9-140">Response</span></span>
<span data-ttu-id="1ecb9-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-141">The following is an example of the response.</span></span>
><span data-ttu-id="1ecb9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ecb9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 144

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->