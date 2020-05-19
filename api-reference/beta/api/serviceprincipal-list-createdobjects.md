---
title: 'servicePrincipalName: listar createdObjects'
description: Recupere uma lista de objetos directoryobject.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e871785a16e543766a7c5938e2b3792133f322ea
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291227"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="b902f-103">servicePrincipalName: listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="b902f-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="b902f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b902f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b902f-105">Recupere uma lista de objetos directoryobject.</span><span class="sxs-lookup"><span data-stu-id="b902f-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b902f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b902f-106">Permissions</span></span>
<span data-ttu-id="b902f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b902f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b902f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b902f-109">Permission type</span></span>      | <span data-ttu-id="b902f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b902f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b902f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b902f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b902f-112">Application. Read. All, Directory. Read. All, Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="b902f-112">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b902f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b902f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b902f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b902f-114">Not supported.</span></span>    |
|<span data-ttu-id="b902f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b902f-115">Application</span></span> | <span data-ttu-id="b902f-116">Application. Read. All, Directory. Read. All, Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b902f-116">Application.Read.All, Directory.Read.All, Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b902f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b902f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b902f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b902f-118">Optional query parameters</span></span>
<span data-ttu-id="b902f-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b902f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b902f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b902f-120">Request headers</span></span>
| <span data-ttu-id="b902f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b902f-121">Name</span></span>           | <span data-ttu-id="b902f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b902f-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b902f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b902f-123">Authorization</span></span>  | <span data-ttu-id="b902f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b902f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b902f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b902f-126">Request body</span></span>
<span data-ttu-id="b902f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b902f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b902f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b902f-128">Response</span></span>

<span data-ttu-id="b902f-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b902f-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="b902f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b902f-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="b902f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b902f-131">Request</span></span>
<span data-ttu-id="b902f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b902f-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```

### <a name="response"></a><span data-ttu-id="b902f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b902f-133">Response</span></span>
<span data-ttu-id="b902f-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b902f-134">Here is an example of the response.</span></span> 
><span data-ttu-id="b902f-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b902f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
