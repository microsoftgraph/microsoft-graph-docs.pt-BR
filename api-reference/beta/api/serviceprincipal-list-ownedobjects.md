---
title: 'servicePrincipals: listar ownedObjects'
description: Recupere uma lista de objetos pertencentes a servicePrincipal.  Isso pode incluir aplicativos ou grupos.
ms.openlocfilehash: 79ca70c5c86e535a7d8a11598509e7ebf61780a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039353"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="06124-104">servicePrincipals: listar ownedObjects</span><span class="sxs-lookup"><span data-stu-id="06124-104">servicePrincipals: List ownedObjects</span></span>

> <span data-ttu-id="06124-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06124-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06124-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06124-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06124-107">Recupere uma lista de objetos pertencentes a servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="06124-107">Retrieve a list of objects owned by the servicePrincipal.</span></span>  <span data-ttu-id="06124-108">Isso pode incluir aplicativos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="06124-108">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="06124-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="06124-109">Permissions</span></span>
<span data-ttu-id="06124-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06124-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06124-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06124-112">Permission type</span></span>      | <span data-ttu-id="06124-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06124-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06124-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06124-114">Delegated (work or school account)</span></span> | <span data-ttu-id="06124-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="06124-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="06124-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06124-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06124-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06124-117">Not supported.</span></span>    |
|<span data-ttu-id="06124-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06124-118">Application</span></span> | <span data-ttu-id="06124-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06124-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06124-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06124-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="06124-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="06124-121">Optional query parameters</span></span>
<span data-ttu-id="06124-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="06124-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06124-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06124-123">Request headers</span></span>
| <span data-ttu-id="06124-124">Nome</span><span class="sxs-lookup"><span data-stu-id="06124-124">Name</span></span>       | <span data-ttu-id="06124-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="06124-125">Type</span></span> | <span data-ttu-id="06124-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="06124-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06124-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="06124-127">Authorization</span></span>  | <span data-ttu-id="06124-128">string</span><span class="sxs-lookup"><span data-stu-id="06124-128">string</span></span>  | <span data-ttu-id="06124-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06124-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06124-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06124-131">Request body</span></span>
<span data-ttu-id="06124-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06124-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06124-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="06124-133">Response</span></span>

<span data-ttu-id="06124-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06124-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06124-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06124-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06124-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06124-136">Request</span></span>
<span data-ttu-id="06124-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06124-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="06124-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="06124-138">Response</span></span>
<span data-ttu-id="06124-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06124-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->