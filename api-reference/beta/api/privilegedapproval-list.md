---
title: Lista privilegedApproval
description: Recupere uma lista de objetos privilegedapproval.
ms.openlocfilehash: 69e558a734f86dd72b35e61d9f8ceab52b9f981e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039583"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="eeb20-103">Lista privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="eeb20-103">List privilegedApproval</span></span>

> <span data-ttu-id="eeb20-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eeb20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eeb20-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eeb20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eeb20-106">Recupere uma lista de objetos privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="eeb20-106">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="eeb20-107">Para filtrar os resultados da consulta, use o OData standard ``$filter`` expressões nos URIs.</span><span class="sxs-lookup"><span data-stu-id="eeb20-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="eeb20-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="eeb20-108">Permissions</span></span>
<span data-ttu-id="eeb20-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eeb20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eeb20-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eeb20-111">Permission type</span></span>      | <span data-ttu-id="eeb20-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eeb20-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeb20-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eeb20-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eeb20-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eeb20-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eeb20-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eeb20-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeb20-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eeb20-116">Not supported.</span></span>    |
|<span data-ttu-id="eeb20-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eeb20-117">Application</span></span> | <span data-ttu-id="eeb20-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eeb20-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeb20-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eeb20-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eeb20-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eeb20-120">Optional query parameters</span></span>
<span data-ttu-id="eeb20-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eeb20-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eeb20-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eeb20-122">Request headers</span></span>
| <span data-ttu-id="eeb20-123">Nome</span><span class="sxs-lookup"><span data-stu-id="eeb20-123">Name</span></span>      |<span data-ttu-id="eeb20-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb20-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eeb20-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="eeb20-125">Authorization</span></span>  | <span data-ttu-id="eeb20-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eeb20-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eeb20-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eeb20-128">Request body</span></span>
<span data-ttu-id="eeb20-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eeb20-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeb20-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeb20-130">Response</span></span>

<span data-ttu-id="eeb20-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eeb20-131">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="eeb20-132">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="eeb20-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="eeb20-133">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="eeb20-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="eeb20-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eeb20-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeb20-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eeb20-135">Request</span></span>
<span data-ttu-id="eeb20-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eeb20-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
##### <a name="response"></a><span data-ttu-id="eeb20-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="eeb20-137">Response</span></span>
<span data-ttu-id="eeb20-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eeb20-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
