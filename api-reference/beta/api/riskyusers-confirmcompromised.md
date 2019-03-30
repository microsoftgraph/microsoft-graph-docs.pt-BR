---
title: Confirmar riskyUsers comprometido
description: Confirme um objeto riskyUsers como comprometido.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 9ae07bf8d1d4a41764aa145a9c7508da339d7ce2
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2019
ms.locfileid: "31013121"
---
# <a name="confirm-riskyusers-compromised"></a><span data-ttu-id="96703-103">Confirmar riskyUsers comprometido</span><span class="sxs-lookup"><span data-stu-id="96703-103">Confirm riskyUsers compromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="96703-104">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="96703-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="96703-105">Confirme um objeto [riskyUsers](../resources/riskyuser.md) como comprometido.</span><span class="sxs-lookup"><span data-stu-id="96703-105">Confirm a [riskyUsers](../resources/riskyuser.md) object as compromised.</span></span> <span data-ttu-id="96703-106">Isso definirá o nível de risco do usuário de destino como alto.</span><span class="sxs-lookup"><span data-stu-id="96703-106">This will set the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="96703-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="96703-107">Permissions</span></span>
<span data-ttu-id="96703-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96703-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96703-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96703-110">Permission type</span></span>      | <span data-ttu-id="96703-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96703-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96703-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96703-112">Delegated (work or school account)</span></span> | <span data-ttu-id="96703-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96703-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="96703-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96703-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96703-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96703-115">Not supported.</span></span>    |
|<span data-ttu-id="96703-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96703-116">Application</span></span> | <span data-ttu-id="96703-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="96703-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96703-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96703-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="96703-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96703-119">Request headers</span></span>
| <span data-ttu-id="96703-120">Nome</span><span class="sxs-lookup"><span data-stu-id="96703-120">Name</span></span>      |<span data-ttu-id="96703-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="96703-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96703-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="96703-122">Authorization</span></span>  | <span data-ttu-id="96703-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96703-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96703-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="96703-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="96703-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="96703-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96703-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96703-128">Request body</span></span>
<span data-ttu-id="96703-129">Especifique as userIds a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96703-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="96703-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="96703-130">Response</span></span>

<span data-ttu-id="96703-131">Se tiver êxito, este método retornará `204 No Content` um código de resposta</span><span class="sxs-lookup"><span data-stu-id="96703-131">If successful, this method returns a `204 No Content` response code</span></span>
## <a name="example"></a><span data-ttu-id="96703-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96703-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96703-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96703-133">Request</span></span>
<span data-ttu-id="96703-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96703-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised


Request Body
{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="96703-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="96703-135">Response</span></span>
<span data-ttu-id="96703-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96703-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 204 NoContent
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
