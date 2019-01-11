---
title: Obter privilegedApproval
description: Recupere as propriedades e relações do objeto privilegedapproval.
localization_priority: Normal
ms.openlocfilehash: eef213416232db67bb0c1134e35d4af94734b468
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847618"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="84d24-103">Obter privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="84d24-103">Get privilegedApproval</span></span>

> <span data-ttu-id="84d24-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="84d24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84d24-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="84d24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84d24-106">Recupere as propriedades e relações do objeto privilegedapproval.</span><span class="sxs-lookup"><span data-stu-id="84d24-106">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="84d24-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="84d24-107">Permissions</span></span>
<span data-ttu-id="84d24-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84d24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="84d24-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84d24-110">Permission type</span></span>      | <span data-ttu-id="84d24-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="84d24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84d24-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84d24-112">Delegated (work or school account)</span></span> | <span data-ttu-id="84d24-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="84d24-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="84d24-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84d24-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84d24-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84d24-115">Not supported.</span></span>    |
|<span data-ttu-id="84d24-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84d24-116">Application</span></span> | <span data-ttu-id="84d24-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84d24-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84d24-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84d24-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="84d24-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="84d24-119">Optional query parameters</span></span>
<span data-ttu-id="84d24-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="84d24-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84d24-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84d24-121">Request headers</span></span>
| <span data-ttu-id="84d24-122">Nome</span><span class="sxs-lookup"><span data-stu-id="84d24-122">Name</span></span>      |<span data-ttu-id="84d24-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="84d24-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="84d24-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="84d24-124">Authorization</span></span>  | <span data-ttu-id="84d24-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84d24-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84d24-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84d24-127">Request body</span></span>
<span data-ttu-id="84d24-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="84d24-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84d24-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="84d24-129">Response</span></span>

<span data-ttu-id="84d24-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84d24-130">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="84d24-131">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="84d24-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="84d24-132">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="84d24-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="84d24-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84d24-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84d24-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84d24-134">Request</span></span>
<span data-ttu-id="84d24-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84d24-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="84d24-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="84d24-136">Response</span></span>
<span data-ttu-id="84d24-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84d24-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
