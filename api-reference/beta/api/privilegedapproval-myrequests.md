---
title: 'privilegedApproval: myRequests'
description: Receba solicitações de aprovação do solicitante.
localization_priority: Normal
ms.openlocfilehash: b894085563abc7c53addb5ad96c90f937e54219d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332071"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="7d85f-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="7d85f-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d85f-104">Receba solicitações de aprovação do solicitante.</span><span class="sxs-lookup"><span data-stu-id="7d85f-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d85f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d85f-105">Permissions</span></span>
<span data-ttu-id="7d85f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d85f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7d85f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d85f-108">Permission type</span></span>      | <span data-ttu-id="7d85f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d85f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d85f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d85f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d85f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d85f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d85f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d85f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d85f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d85f-113">Not supported.</span></span>    |
|<span data-ttu-id="7d85f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d85f-114">Application</span></span> | <span data-ttu-id="7d85f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d85f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d85f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d85f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="7d85f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d85f-117">Request headers</span></span>
| <span data-ttu-id="7d85f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7d85f-118">Name</span></span>       | <span data-ttu-id="7d85f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d85f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7d85f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d85f-120">Authorization</span></span>  | <span data-ttu-id="7d85f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d85f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d85f-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d85f-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7d85f-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d85f-124">Response</span></span>

<span data-ttu-id="7d85f-125">Se bem-sucedido, este método retorna `200 OK` o código de resposta e o objeto [privilegedApproval](../resources/privilegedapproval.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d85f-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="7d85f-126">Observe que o locatário precisa ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="7d85f-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7d85f-127">Caso contrário, o código de status HTTP 403 proibido será retornado.</span><span class="sxs-lookup"><span data-stu-id="7d85f-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="7d85f-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d85f-128">Example</span></span>
<span data-ttu-id="7d85f-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7d85f-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7d85f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d85f-130">Request</span></span>
<span data-ttu-id="7d85f-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d85f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```

##### <a name="response"></a><span data-ttu-id="7d85f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d85f-132">Response</span></span>
<span data-ttu-id="7d85f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7d85f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
