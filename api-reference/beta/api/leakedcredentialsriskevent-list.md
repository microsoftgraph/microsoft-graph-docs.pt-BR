---
title: Listar leakedCredentialsRiskEvents
description: Recupere uma lista de objetos leakedcredentialsriskevent.
localization_priority: Normal
ms.openlocfilehash: ad34b75117c33014f76464ed85d5f4a644d1de8e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541035"
---
# <a name="list-leakedcredentialsriskevents"></a><span data-ttu-id="af7d8-103">Listar leakedCredentialsRiskEvents</span><span class="sxs-lookup"><span data-stu-id="af7d8-103">List leakedCredentialsRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af7d8-104">Recupere uma lista de objetos leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="af7d8-104">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="af7d8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="af7d8-105">Permissions</span></span>
<span data-ttu-id="af7d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af7d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af7d8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af7d8-108">Permission type</span></span>      | <span data-ttu-id="af7d8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af7d8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af7d8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af7d8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af7d8-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="af7d8-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="af7d8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af7d8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af7d8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af7d8-113">Not supported.</span></span>    |
|<span data-ttu-id="af7d8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af7d8-114">Application</span></span> | <span data-ttu-id="af7d8-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="af7d8-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af7d8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af7d8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="af7d8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af7d8-117">Request headers</span></span>
| <span data-ttu-id="af7d8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="af7d8-118">Name</span></span>      |<span data-ttu-id="af7d8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="af7d8-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="af7d8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="af7d8-120">Authorization</span></span>  | <span data-ttu-id="af7d8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af7d8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="af7d8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="af7d8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="af7d8-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="af7d8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af7d8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af7d8-126">Request body</span></span>
<span data-ttu-id="af7d8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af7d8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af7d8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="af7d8-128">Response</span></span>

<span data-ttu-id="af7d8-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af7d8-129">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="af7d8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af7d8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af7d8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af7d8-131">Request</span></span>
<span data-ttu-id="af7d8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af7d8-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="af7d8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="af7d8-133">Response</span></span>
<span data-ttu-id="af7d8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af7d8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value":
  [
    {
      "closedDateTime": null,
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "active",
      "riskLevel": "high",
      "riskType": "LeakedCredentialsRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/leakedcredentialsriskevent-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
