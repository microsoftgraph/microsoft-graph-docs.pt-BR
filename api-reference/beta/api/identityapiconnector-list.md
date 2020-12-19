---
title: Listar identityApiConnectors
description: Obter uma lista dos objetos identityApiConnector e suas propriedades
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ca946e80b590926aa8f15b7b790d5bd098838cf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720077"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="f8255-103">Listar identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="f8255-103">List identityApiConnectors</span></span>

<span data-ttu-id="f8255-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8255-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8255-105">Ler as propriedades de um objeto [identityApiConnector](../resources/identityapiconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="f8255-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8255-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8255-106">Permissions</span></span>

<span data-ttu-id="f8255-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8255-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8255-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8255-109">Permission type</span></span>                        | <span data-ttu-id="f8255-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8255-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f8255-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8255-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8255-112">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f8255-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="f8255-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8255-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8255-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8255-114">Not supported.</span></span>  |
| <span data-ttu-id="f8255-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8255-115">Application</span></span>                            | <span data-ttu-id="f8255-116">APIConnectors. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f8255-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="f8255-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="f8255-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f8255-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f8255-118">Global administrator</span></span>
* <span data-ttu-id="f8255-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="f8255-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f8255-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8255-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8255-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f8255-121">Optional query parameters</span></span>
<span data-ttu-id="f8255-122">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f8255-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f8255-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f8255-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8255-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8255-124">Request headers</span></span>
|<span data-ttu-id="f8255-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f8255-125">Name</span></span>|<span data-ttu-id="f8255-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8255-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8255-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8255-127">Authorization</span></span>|<span data-ttu-id="f8255-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8255-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8255-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8255-130">Request body</span></span>
<span data-ttu-id="f8255-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8255-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8255-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8255-132">Response</span></span>

<span data-ttu-id="f8255-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [identityApiConnector](../resources/identityapiconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8255-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8255-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8255-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8255-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8255-135">Request</span></span>

<span data-ttu-id="f8255-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8255-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```

### <a name="response"></a><span data-ttu-id="f8255-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8255-137">Response</span></span>

<span data-ttu-id="f8255-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f8255-138">The following is an example of the response.</span></span>

<span data-ttu-id="f8255-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f8255-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors",
    "value": [
      {
          "id": "<guid>",
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
