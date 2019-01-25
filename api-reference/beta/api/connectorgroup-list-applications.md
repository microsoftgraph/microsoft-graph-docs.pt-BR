---
title: Lista de aplicativos
description: Recupere uma lista de objetos de aplicativos associados a connectorGroup.
localization_priority: Normal
ms.openlocfilehash: 47be81d4f154d87865113fa02b04a58151545507
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519357"
---
# <a name="list-applications"></a><span data-ttu-id="90fc7-103">Lista de aplicativos</span><span class="sxs-lookup"><span data-stu-id="90fc7-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90fc7-104">Recupere uma lista de objetos de aplicativos associados a connectorGroup.</span><span class="sxs-lookup"><span data-stu-id="90fc7-104">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="90fc7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="90fc7-105">Permissions</span></span>
<span data-ttu-id="90fc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90fc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90fc7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90fc7-108">Permission type</span></span>      | <span data-ttu-id="90fc7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="90fc7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90fc7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90fc7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90fc7-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90fc7-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90fc7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90fc7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90fc7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90fc7-113">Not supported.</span></span>    |
|<span data-ttu-id="90fc7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="90fc7-114">Application</span></span> | <span data-ttu-id="90fc7-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90fc7-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90fc7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90fc7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="90fc7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="90fc7-117">Optional query parameters</span></span>
<span data-ttu-id="90fc7-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="90fc7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90fc7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90fc7-119">Request headers</span></span>
| <span data-ttu-id="90fc7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="90fc7-120">Name</span></span>      |<span data-ttu-id="90fc7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="90fc7-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90fc7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="90fc7-122">Authorization</span></span>  | <span data-ttu-id="90fc7-123"> de portador</span><span class="sxs-lookup"><span data-stu-id="90fc7-123">Bearer.</span></span> <span data-ttu-id="90fc7-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="90fc7-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="90fc7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90fc7-125">Request body</span></span>
<span data-ttu-id="90fc7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="90fc7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90fc7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="90fc7-127">Response</span></span>

<span data-ttu-id="90fc7-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos de [aplicativo](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90fc7-128">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="90fc7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90fc7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90fc7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90fc7-130">Request</span></span>
<span data-ttu-id="90fc7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90fc7-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="90fc7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="90fc7-132">Response</span></span>
<span data-ttu-id="90fc7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90fc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
    {
      "appId": "appId-value",
      "onPremisesPublishing": {
        "externalUrl": "externalUrl-value",
        "internalUrl": "internalUrl-value",
        "externalAuthenticationType": "externalAuthenticationType-value",
        "customDomainCertificate": "customDomainCertificate-value",
        "isTranslateHostHeaderEnabled": true,
        "isOnPremPublishingEnabled": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-list-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
