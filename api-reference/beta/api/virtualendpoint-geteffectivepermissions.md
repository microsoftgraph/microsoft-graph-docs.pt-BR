---
title: 'virtualEndpoint: getEffectivePermissions'
description: '**GetEffectivePermissions é uma função que Retrives as permissões efetivas do usuário atualmente autenticado, o que ajuda o UX a ocultar ou desabilitar o conteúdo ao qual o usuário atual não tem acesso.**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e87deb3bafbcd1ac28a1d95209f62017d7593e6c
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714344"
---
# <a name="virtualendpoint-geteffectivepermissions"></a><span data-ttu-id="27002-103">virtualEndpoint: getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="27002-103">virtualEndpoint: getEffectivePermissions</span></span>

<span data-ttu-id="27002-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27002-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27002-105">Exibir as permissões efetivas do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="27002-105">View the effective permissions of the currently authenticated user.</span></span> <span data-ttu-id="27002-106">GetEffectivePermissions é uma função que Retrives as permissões efetivas do usuário atualmente autenticado, o que ajuda o UX a ocultar ou desabilitar o conteúdo ao qual o usuário atual não tem acesso.</span><span class="sxs-lookup"><span data-stu-id="27002-106">GetEffectivePermissions is a function that retrives the effective permissions of the currently authenticated user, which helps UX hide or disable content that the current user doesn't have access to.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="27002-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="27002-107">Permissions</span></span>

<span data-ttu-id="27002-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27002-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27002-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27002-110">Permission type</span></span>|<span data-ttu-id="27002-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27002-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27002-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27002-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27002-113">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="27002-113">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="27002-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27002-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27002-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27002-115">Not supported.</span></span>|
|<span data-ttu-id="27002-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27002-116">Application</span></span>| <span data-ttu-id="27002-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27002-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27002-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27002-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="27002-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27002-119">Request headers</span></span>

| <span data-ttu-id="27002-120">Nome</span><span class="sxs-lookup"><span data-stu-id="27002-120">Name</span></span>          | <span data-ttu-id="27002-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="27002-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="27002-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="27002-122">Authorization</span></span> | <span data-ttu-id="27002-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27002-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27002-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27002-125">Request body</span></span>

<span data-ttu-id="27002-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27002-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27002-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="27002-127">Response</span></span>

<span data-ttu-id="27002-128">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27002-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span> <span data-ttu-id="27002-129">Se o usuário tiver permissões completas, a resposta será `["*"]` .</span><span class="sxs-lookup"><span data-stu-id="27002-129">If the user has full permissions, the response is `["*"]`.</span></span>

## <a name="examples"></a><span data-ttu-id="27002-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27002-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27002-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27002-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="27002-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="27002-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```
# <a name="c"></a>[<span data-ttu-id="27002-133">C#</span><span class="sxs-lookup"><span data-stu-id="27002-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/virtualendpoint-geteffectivepermissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27002-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27002-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/virtualendpoint-geteffectivepermissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27002-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27002-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/virtualendpoint-geteffectivepermissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27002-136">Java</span><span class="sxs-lookup"><span data-stu-id="27002-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/virtualendpoint-geteffectivepermissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27002-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="27002-137">Response</span></span>

<span data-ttu-id="27002-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27002-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      "Microsoft.CloudPC/CloudPCs/Read"
   ]
}
```
