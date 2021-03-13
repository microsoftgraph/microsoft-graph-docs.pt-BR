---
title: Obter printSettings
description: Recupere as configurações de todo o locatário para o serviço de Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 4be764fc6ace444669a6d0c0a72047a41c9feab2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777233"
---
# <a name="get-printsettings"></a><span data-ttu-id="cbd39-103">Obter printSettings</span><span class="sxs-lookup"><span data-stu-id="cbd39-103">Get printSettings</span></span>

<span data-ttu-id="cbd39-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbd39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="cbd39-105">Recupere as configurações de todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="cbd39-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbd39-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cbd39-106">Permissions</span></span>
<span data-ttu-id="cbd39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbd39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cbd39-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="cbd39-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="cbd39-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="cbd39-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="cbd39-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cbd39-111">Permission type</span></span> | <span data-ttu-id="cbd39-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cbd39-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="cbd39-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cbd39-113">Delegated (work or school account)</span></span>| <span data-ttu-id="cbd39-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbd39-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="cbd39-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cbd39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbd39-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbd39-116">Not Supported.</span></span>|
|<span data-ttu-id="cbd39-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cbd39-117">Application</span></span>|<span data-ttu-id="cbd39-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cbd39-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbd39-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cbd39-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbd39-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cbd39-120">Optional query parameters</span></span>
<span data-ttu-id="cbd39-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cbd39-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cbd39-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cbd39-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbd39-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd39-123">Request headers</span></span>
| <span data-ttu-id="cbd39-124">Nome</span><span class="sxs-lookup"><span data-stu-id="cbd39-124">Name</span></span>      |<span data-ttu-id="cbd39-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbd39-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cbd39-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="cbd39-126">Authorization</span></span> | <span data-ttu-id="cbd39-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cbd39-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbd39-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd39-129">Request body</span></span>
<span data-ttu-id="cbd39-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cbd39-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbd39-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbd39-131">Response</span></span>
<span data-ttu-id="cbd39-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printSettings](../resources/printsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cbd39-132">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cbd39-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cbd39-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cbd39-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cbd39-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cbd39-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="cbd39-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/settings
```
# <a name="c"></a>[<span data-ttu-id="cbd39-136">C#</span><span class="sxs-lookup"><span data-stu-id="cbd39-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cbd39-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cbd39-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cbd39-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cbd39-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cbd39-139">Java</span><span class="sxs-lookup"><span data-stu-id="cbd39-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cbd39-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="cbd39-140">Response</span></span>
<span data-ttu-id="cbd39-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cbd39-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

