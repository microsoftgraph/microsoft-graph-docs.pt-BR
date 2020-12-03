---
title: 'virtualEndpoint: getEffectivePermissions'
description: '**GetEffectivePermissions é uma função que Retrives as permissões efetivas do usuário atualmente autenticado, o que ajuda o UX a ocultar ou desabilitar o conteúdo ao qual o usuário atual não tem acesso.**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: df6d0ffbdffdf01c30f5dda2220cc96392b0f6ed
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563899"
---
# <a name="virtualendpoint-geteffectivepermissions"></a><span data-ttu-id="021f5-103">virtualEndpoint: getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="021f5-103">virtualEndpoint: getEffectivePermissions</span></span>

<span data-ttu-id="021f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="021f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="021f5-105">Exibir as permissões efetivas do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="021f5-105">View the effective permissions of the currently authenticated user.</span></span> <span data-ttu-id="021f5-106">GetEffectivePermissions é uma função que Retrives as permissões efetivas do usuário atualmente autenticado, o que ajuda o UX a ocultar ou desabilitar o conteúdo ao qual o usuário atual não tem acesso.</span><span class="sxs-lookup"><span data-stu-id="021f5-106">GetEffectivePermissions is a function that retrives the effective permissions of the currently authenticated user, which helps UX hide or disable content that the current user doesn't have access to.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="021f5-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="021f5-107">Permissions</span></span>

<span data-ttu-id="021f5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="021f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="021f5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="021f5-110">Permission type</span></span>|<span data-ttu-id="021f5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="021f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="021f5-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="021f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="021f5-113">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="021f5-113">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="021f5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="021f5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="021f5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="021f5-115">Not supported.</span></span>|
|<span data-ttu-id="021f5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="021f5-116">Application</span></span>| <span data-ttu-id="021f5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="021f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="021f5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="021f5-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="021f5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="021f5-119">Request headers</span></span>

| <span data-ttu-id="021f5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="021f5-120">Name</span></span>          | <span data-ttu-id="021f5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="021f5-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="021f5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="021f5-122">Authorization</span></span> | <span data-ttu-id="021f5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="021f5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="021f5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="021f5-125">Request body</span></span>

<span data-ttu-id="021f5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="021f5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="021f5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="021f5-127">Response</span></span>

<span data-ttu-id="021f5-128">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="021f5-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span> <span data-ttu-id="021f5-129">Se o usuário tiver permissões completas, a resposta será `["*"]` .</span><span class="sxs-lookup"><span data-stu-id="021f5-129">If the user has full permissions, the response is `["*"]`.</span></span>

## <a name="examples"></a><span data-ttu-id="021f5-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="021f5-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="021f5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="021f5-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="021f5-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="021f5-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```
# <a name="c"></a>[<span data-ttu-id="021f5-133">C#</span><span class="sxs-lookup"><span data-stu-id="021f5-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/virtualendpoint-geteffectivepermissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="021f5-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="021f5-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/virtualendpoint-geteffectivepermissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="021f5-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="021f5-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/virtualendpoint-geteffectivepermissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="021f5-136">Java</span><span class="sxs-lookup"><span data-stu-id="021f5-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/virtualendpoint-geteffectivepermissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="021f5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="021f5-137">Response</span></span>

<span data-ttu-id="021f5-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="021f5-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    "Microsoft.CloudPC/CloudPCs/Read"
  ]
}
```
