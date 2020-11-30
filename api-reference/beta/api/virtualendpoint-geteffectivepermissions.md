---
title: 'virtualEndpoint: getEffectivePermissions'
description: '**GetEffectivePermissions é uma função que Retrives as permissões efetivas do usuário atualmente autenticado, o que ajuda o UX a ocultar ou desabilitar o conteúdo ao qual o usuário atual não tem acesso.**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 78b58c5ea00e1b170d831a91f5dc3ff1569bd0d7
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378261"
---
# <a name="virtualendpoint-geteffectivepermissions"></a><span data-ttu-id="5449d-103">virtualEndpoint: getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="5449d-103">virtualEndpoint: getEffectivePermissions</span></span>

<span data-ttu-id="5449d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5449d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5449d-105">Exibir as permissões efetivas do usuário autenticado no momento.</span><span class="sxs-lookup"><span data-stu-id="5449d-105">View the effective permissions of the currently authenticated user.</span></span> <span data-ttu-id="5449d-106">GetEffectivePermissions é uma função que Retrives as permissões efetivas do usuário atualmente autenticado, o que ajuda o UX a ocultar ou desabilitar o conteúdo ao qual o usuário atual não tem acesso.</span><span class="sxs-lookup"><span data-stu-id="5449d-106">GetEffectivePermissions is a function that retrives the effective permissions of the currently authenticated user, which helps UX hide or disable content that the current user doesn't have access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="5449d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="5449d-107">Permissions</span></span>

<span data-ttu-id="5449d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5449d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5449d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5449d-110">Permission type</span></span>|<span data-ttu-id="5449d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5449d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5449d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5449d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5449d-113">CloudPC. ReadWrite. All, CloudPC. Read. All</span><span class="sxs-lookup"><span data-stu-id="5449d-113">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="5449d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5449d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5449d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5449d-115">Not supported.</span></span>|
|<span data-ttu-id="5449d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5449d-116">Application</span></span>| <span data-ttu-id="5449d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5449d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5449d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5449d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="5449d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5449d-119">Request headers</span></span>

| <span data-ttu-id="5449d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5449d-120">Name</span></span>          | <span data-ttu-id="5449d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5449d-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5449d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5449d-122">Authorization</span></span> | <span data-ttu-id="5449d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5449d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5449d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5449d-125">Request body</span></span>

<span data-ttu-id="5449d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5449d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5449d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5449d-127">Response</span></span>

<span data-ttu-id="5449d-128">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5449d-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span> <span data-ttu-id="5449d-129">Se o usuário tiver permissões completas, a resposta será `["*"]` .</span><span class="sxs-lookup"><span data-stu-id="5449d-129">If the user has full permissions, the response is `["*"]`.</span></span>

## <a name="examples"></a><span data-ttu-id="5449d-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5449d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5449d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5449d-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```

### <a name="response"></a><span data-ttu-id="5449d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5449d-132">Response</span></span>

<span data-ttu-id="5449d-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5449d-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
