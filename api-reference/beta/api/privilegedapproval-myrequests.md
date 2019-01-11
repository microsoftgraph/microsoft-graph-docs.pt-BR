---
title: 'privilegedApproval: myRequests'
description: Obtenha as solicitações de aprovação do solicitador.
localization_priority: Normal
ms.openlocfilehash: 26c8805d669b5786ac2c46821570f6cd29a99f2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806409"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="29c4d-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="29c4d-103">privilegedApproval: myRequests</span></span>

> <span data-ttu-id="29c4d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="29c4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29c4d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="29c4d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="29c4d-106">Obtenha as solicitações de aprovação do solicitador.</span><span class="sxs-lookup"><span data-stu-id="29c4d-106">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="29c4d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="29c4d-107">Permissions</span></span>
<span data-ttu-id="29c4d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29c4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="29c4d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29c4d-110">Permission type</span></span>      | <span data-ttu-id="29c4d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29c4d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29c4d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29c4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29c4d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29c4d-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29c4d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29c4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29c4d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c4d-115">Not supported.</span></span>    |
|<span data-ttu-id="29c4d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29c4d-116">Application</span></span> | <span data-ttu-id="29c4d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29c4d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29c4d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29c4d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="29c4d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29c4d-119">Request headers</span></span>
| <span data-ttu-id="29c4d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="29c4d-120">Name</span></span>       | <span data-ttu-id="29c4d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="29c4d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29c4d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="29c4d-122">Authorization</span></span>  | <span data-ttu-id="29c4d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29c4d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29c4d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29c4d-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="29c4d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c4d-126">Response</span></span>

<span data-ttu-id="29c4d-127">Se tiver êxito, este método retornará `200 OK` objeto response de código e [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29c4d-127">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="29c4d-128">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="29c4d-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="29c4d-129">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="29c4d-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="29c4d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29c4d-130">Example</span></span>
<span data-ttu-id="29c4d-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="29c4d-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29c4d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29c4d-132">Request</span></span>
<span data-ttu-id="29c4d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29c4d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="29c4d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="29c4d-134">Response</span></span>
<span data-ttu-id="29c4d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29c4d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
