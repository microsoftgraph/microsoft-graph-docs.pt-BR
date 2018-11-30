---
title: 'servicePrincipal: listar createdObjects'
description: Recupere uma lista de objetos directoryobject.
ms.openlocfilehash: 406d9bd18c662d00fd4e4ddb17598454197676b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036315"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="3f2f0-103">servicePrincipal: listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="3f2f0-103">servicePrincipal: List createdObjects</span></span>

> <span data-ttu-id="3f2f0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f2f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f2f0-106">Recupere uma lista de objetos directoryobject.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-106">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f2f0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3f2f0-107">Permissions</span></span>
<span data-ttu-id="3f2f0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f2f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f2f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f2f0-110">Permission type</span></span>      | <span data-ttu-id="3f2f0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f2f0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f2f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f2f0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3f2f0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f2f0-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f2f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f2f0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f2f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-115">Not supported.</span></span>    |
|<span data-ttu-id="3f2f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3f2f0-116">Application</span></span> | <span data-ttu-id="3f2f0-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f2f0-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f2f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f2f0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3f2f0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3f2f0-119">Optional query parameters</span></span>
<span data-ttu-id="3f2f0-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f2f0-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f2f0-121">Request headers</span></span>
| <span data-ttu-id="3f2f0-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3f2f0-122">Name</span></span>       | <span data-ttu-id="3f2f0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f2f0-123">Type</span></span> | <span data-ttu-id="3f2f0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f2f0-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3f2f0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f2f0-125">Authorization</span></span>  | <span data-ttu-id="3f2f0-126">string</span><span class="sxs-lookup"><span data-stu-id="3f2f0-126">string</span></span>  | <span data-ttu-id="3f2f0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f2f0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f2f0-129">Request body</span></span>
<span data-ttu-id="3f2f0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f2f0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f2f0-131">Response</span></span>

<span data-ttu-id="3f2f0-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3f2f0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3f2f0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f2f0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f2f0-134">Request</span></span>
<span data-ttu-id="3f2f0-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
##### <a name="response"></a><span data-ttu-id="3f2f0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f2f0-136">Response</span></span>
<span data-ttu-id="3f2f0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3f2f0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->