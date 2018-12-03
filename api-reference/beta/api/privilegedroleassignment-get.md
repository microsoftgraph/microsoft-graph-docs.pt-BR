---
title: Obter privilegedRoleAssignment
description: Recupere as propriedades e relações do objeto privilegedRoleAssignment.
ms.openlocfilehash: ad8815842698be0ef6a3eef37dc3e26f7dc11dbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035367"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="ea7d8-103">Obter privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ea7d8-103">Get privilegedRoleAssignment</span></span>

> <span data-ttu-id="ea7d8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea7d8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ea7d8-106">Recupere as propriedades e relações do objeto privilegedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-106">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea7d8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ea7d8-107">Permissions</span></span>
<span data-ttu-id="ea7d8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea7d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ea7d8-110">O solicitante precisa ter uma das seguintes funções: _Leitor de segurança_, _Administrador Global_, _Administrador de segurança_ou _Administrador com privilégios de função_.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="ea7d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea7d8-111">Permission type</span></span>      | <span data-ttu-id="ea7d8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea7d8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea7d8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea7d8-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ea7d8-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea7d8-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea7d8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea7d8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea7d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-116">Not supported.</span></span>    |
|<span data-ttu-id="ea7d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea7d8-117">Application</span></span> | <span data-ttu-id="ea7d8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea7d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea7d8-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea7d8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ea7d8-120">Optional query parameters</span></span>
<span data-ttu-id="ea7d8-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea7d8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea7d8-122">Request headers</span></span>
| <span data-ttu-id="ea7d8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ea7d8-123">Name</span></span>      |<span data-ttu-id="ea7d8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea7d8-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ea7d8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea7d8-125">Authorization</span></span>  | <span data-ttu-id="ea7d8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea7d8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea7d8-128">Request body</span></span>
<span data-ttu-id="ea7d8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea7d8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea7d8-130">Response</span></span>

<span data-ttu-id="ea7d8-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [privilegedRoleAssignment](../resources/privilegedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-131">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="ea7d8-132">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ea7d8-133">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ea7d8-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea7d8-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea7d8-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea7d8-135">Request</span></span>
<span data-ttu-id="ea7d8-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="ea7d8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea7d8-137">Response</span></span>
<span data-ttu-id="ea7d8-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea7d8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->