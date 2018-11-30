---
title: Obter privilegedApproval
description: Recupere as propriedades e relações do objeto privilegedapproval.
ms.openlocfilehash: 77db18f46bbdfec6a5a9a62e4e481facaab6cb8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039141"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="cb752-103">Obter privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="cb752-103">Get privilegedApproval</span></span>

> <span data-ttu-id="cb752-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cb752-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb752-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cb752-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb752-106">Recupere as propriedades e relações do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="cb752-106">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cb752-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="cb752-107">Permissions</span></span>
<span data-ttu-id="cb752-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb752-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cb752-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb752-110">Permission type</span></span>      | <span data-ttu-id="cb752-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb752-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb752-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb752-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cb752-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cb752-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cb752-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb752-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb752-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb752-115">Not supported.</span></span>    |
|<span data-ttu-id="cb752-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb752-116">Application</span></span> | <span data-ttu-id="cb752-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb752-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb752-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb752-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb752-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cb752-119">Optional query parameters</span></span>
<span data-ttu-id="cb752-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cb752-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb752-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb752-121">Request headers</span></span>
| <span data-ttu-id="cb752-122">Nome</span><span class="sxs-lookup"><span data-stu-id="cb752-122">Name</span></span>      |<span data-ttu-id="cb752-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb752-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb752-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb752-124">Authorization</span></span>  | <span data-ttu-id="cb752-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb752-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb752-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb752-127">Request body</span></span>
<span data-ttu-id="cb752-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb752-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb752-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb752-129">Response</span></span>

<span data-ttu-id="cb752-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb752-130">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="cb752-131">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="cb752-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cb752-132">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="cb752-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="cb752-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb752-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb752-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb752-134">Request</span></span>
<span data-ttu-id="cb752-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb752-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="cb752-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb752-136">Response</span></span>
<span data-ttu-id="cb752-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb752-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
