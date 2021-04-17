---
title: Listar identityApiConnectors
description: Obter uma lista dos objetos identityApiConnector e suas propriedades.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0417726431261cd25fdc9ee5b58f7fbee8c9d7cd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882766"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="fdb07-103">Listar identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="fdb07-103">List identityApiConnectors</span></span>

<span data-ttu-id="fdb07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdb07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fdb07-105">Leia as propriedades de [um objeto identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="fdb07-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fdb07-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdb07-106">Permissions</span></span>

<span data-ttu-id="fdb07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdb07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fdb07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdb07-109">Permission type</span></span>                        | <span data-ttu-id="fdb07-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdb07-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fdb07-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdb07-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fdb07-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb07-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="fdb07-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdb07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdb07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdb07-114">Not supported.</span></span>  |
| <span data-ttu-id="fdb07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdb07-115">Application</span></span>                            | <span data-ttu-id="fdb07-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb07-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="fdb07-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="fdb07-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="fdb07-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fdb07-118">Global administrator</span></span>
* <span data-ttu-id="fdb07-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="fdb07-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="fdb07-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdb07-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdb07-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fdb07-121">Optional query parameters</span></span>

<span data-ttu-id="fdb07-122">Você pode usar `$expand` para expandir propriedades específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="fdb07-122">You can use `$expand` to expand specific properties that are not expanded by default.</span></span> <span data-ttu-id="fdb07-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fdb07-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdb07-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb07-124">Request headers</span></span>

|<span data-ttu-id="fdb07-125">Nome</span><span class="sxs-lookup"><span data-stu-id="fdb07-125">Name</span></span>|<span data-ttu-id="fdb07-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdb07-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fdb07-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdb07-127">Authorization</span></span>|<span data-ttu-id="fdb07-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdb07-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdb07-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb07-130">Request body</span></span>

<span data-ttu-id="fdb07-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdb07-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdb07-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb07-132">Response</span></span>

<span data-ttu-id="fdb07-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdb07-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdb07-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdb07-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdb07-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb07-135">Request</span></span>

<span data-ttu-id="fdb07-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdb07-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/apiConnectors
```

### <a name="response"></a><span data-ttu-id="fdb07-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb07-137">Response</span></span>

<span data-ttu-id="fdb07-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fdb07-138">The following is an example of the response.</span></span>

<span data-ttu-id="fdb07-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fdb07-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors",
    "value": [
      {
          "id": "be1f769b-9b13-437e-b540-79a905c4932c",
          "displayName": "Test API",
          "targetUrl": "https://someapi.com/api/endpoint",
          "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME>",
            "password": "******"
          }
      }
   ]
}
```
