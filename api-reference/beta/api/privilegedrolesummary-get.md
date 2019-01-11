---
title: Obter privilegedRoleSummary
description: Recupere as propriedades e relações do objeto privilegedRoleSummary.
localization_priority: Normal
ms.openlocfilehash: ebe3a0774869c09ba26cd01726590a6b7cddb58f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816076"
---
# <a name="get-privilegedrolesummary"></a><span data-ttu-id="d263e-103">Obter privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="d263e-103">Get privilegedRoleSummary</span></span>

> <span data-ttu-id="d263e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d263e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d263e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d263e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d263e-106">Recupere as propriedades e relações do objeto [privilegedRoleSummary](../resources/privilegedrolesummary.md) .</span><span class="sxs-lookup"><span data-stu-id="d263e-106">Retrieve the properties and relationships of [privilegedRoleSummary](../resources/privilegedrolesummary.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d263e-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="d263e-107">Permissions</span></span>
<span data-ttu-id="d263e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d263e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d263e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d263e-110">Permission type</span></span>      | <span data-ttu-id="d263e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d263e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d263e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d263e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d263e-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d263e-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d263e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d263e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d263e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d263e-115">Not supported.</span></span>    |
|<span data-ttu-id="d263e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d263e-116">Application</span></span> | <span data-ttu-id="d263e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d263e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d263e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d263e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}?$expand=summary
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d263e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d263e-119">Optional query parameters</span></span>
<span data-ttu-id="d263e-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d263e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d263e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d263e-121">Request headers</span></span>
| <span data-ttu-id="d263e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d263e-122">Name</span></span>      |<span data-ttu-id="d263e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d263e-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d263e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d263e-124">Authorization</span></span>  | <span data-ttu-id="d263e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d263e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d263e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d263e-127">Request body</span></span>
<span data-ttu-id="d263e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d263e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d263e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d263e-129">Response</span></span>

<span data-ttu-id="d263e-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [privilegedRoleSummary](../resources/privilegedrolesummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d263e-130">If successful, this method returns a `200 OK` response code and [privilegedRoleSummary](../resources/privilegedrolesummary.md) object in the response body.</span></span>

<span data-ttu-id="d263e-131">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="d263e-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d263e-132">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="d263e-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d263e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d263e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d263e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d263e-134">Request</span></span>
<span data-ttu-id="d263e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d263e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrolesummary"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/summary
```
##### <a name="response"></a><span data-ttu-id="d263e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d263e-136">Response</span></span>
<span data-ttu-id="d263e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d263e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 137

{
  "id": "id-value",
  "status": "status-value",
  "usersCount": 99,
  "managedCount": 99,
  "elevatedCount": 99,
  "mfaEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
