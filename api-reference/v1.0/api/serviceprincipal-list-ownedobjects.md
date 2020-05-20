---
title: 'servicePrincipalName: listar ownedObjects'
description: Recupere uma lista de objetos pertencentes ao servicePrincipalName.  Isso pode incluir aplicativos ou grupos.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: e790368a9d6b2122174517adf5190c8c3440a556
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291101"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="f06d7-104">servicePrincipalName: listar ownedObjects</span><span class="sxs-lookup"><span data-stu-id="f06d7-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="f06d7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f06d7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f06d7-106">Recupere uma lista de objetos pertencentes ao [servicePrincipalName](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="f06d7-106">Retrieve a list of objects owned by the [servicePrincipal](../resources/serviceprincipal.md).</span></span>  <span data-ttu-id="f06d7-107">Isso pode incluir aplicativos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="f06d7-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="f06d7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f06d7-108">Permissions</span></span>
<span data-ttu-id="f06d7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f06d7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f06d7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f06d7-111">Permission type</span></span>      | <span data-ttu-id="f06d7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f06d7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f06d7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f06d7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f06d7-114">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f06d7-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f06d7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f06d7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f06d7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f06d7-116">Not supported.</span></span>    |
|<span data-ttu-id="f06d7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f06d7-117">Application</span></span> | <span data-ttu-id="f06d7-118">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f06d7-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f06d7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f06d7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f06d7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f06d7-120">Optional query parameters</span></span>
<span data-ttu-id="f06d7-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f06d7-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f06d7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f06d7-122">Request headers</span></span>
| <span data-ttu-id="f06d7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f06d7-123">Name</span></span>           | <span data-ttu-id="f06d7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f06d7-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f06d7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f06d7-125">Authorization</span></span>  | <span data-ttu-id="f06d7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f06d7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f06d7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f06d7-128">Request body</span></span>
<span data-ttu-id="f06d7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f06d7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f06d7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f06d7-130">Response</span></span>

<span data-ttu-id="f06d7-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f06d7-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="f06d7-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f06d7-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f06d7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f06d7-133">Request</span></span>
<span data-ttu-id="f06d7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f06d7-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/ownedObjects
```

### <a name="response"></a><span data-ttu-id="f06d7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f06d7-135">Response</span></span>
<span data-ttu-id="f06d7-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f06d7-136">Here is an example of the response.</span></span> 
><span data-ttu-id="f06d7-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f06d7-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
