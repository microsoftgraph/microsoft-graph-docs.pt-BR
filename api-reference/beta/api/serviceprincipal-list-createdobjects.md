---
title: 'servicePrincipal: listar createdObjects'
description: Recupere uma lista de objetos directoryobject.
localization_priority: Normal
ms.openlocfilehash: 8a20a6812cc94e58471dc9b4afe754da45bf199b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524251"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="669d9-103">servicePrincipal: listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="669d9-103">servicePrincipal: List createdObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="669d9-104">Recupere uma lista de objetos directoryobject.</span><span class="sxs-lookup"><span data-stu-id="669d9-104">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="669d9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="669d9-105">Permissions</span></span>
<span data-ttu-id="669d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="669d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="669d9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="669d9-108">Permission type</span></span>      | <span data-ttu-id="669d9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="669d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="669d9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="669d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="669d9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="669d9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="669d9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="669d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="669d9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="669d9-113">Not supported.</span></span>    |
|<span data-ttu-id="669d9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="669d9-114">Application</span></span> | <span data-ttu-id="669d9-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="669d9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="669d9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="669d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="669d9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="669d9-117">Optional query parameters</span></span>
<span data-ttu-id="669d9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="669d9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="669d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="669d9-119">Request headers</span></span>
| <span data-ttu-id="669d9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="669d9-120">Name</span></span>       | <span data-ttu-id="669d9-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="669d9-121">Type</span></span> | <span data-ttu-id="669d9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="669d9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="669d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="669d9-123">Authorization</span></span>  | <span data-ttu-id="669d9-124">string</span><span class="sxs-lookup"><span data-stu-id="669d9-124">string</span></span>  | <span data-ttu-id="669d9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="669d9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="669d9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="669d9-127">Request body</span></span>
<span data-ttu-id="669d9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="669d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="669d9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="669d9-129">Response</span></span>

<span data-ttu-id="669d9-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="669d9-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="669d9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="669d9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="669d9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="669d9-132">Request</span></span>
<span data-ttu-id="669d9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="669d9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/createdObjects
```
##### <a name="response"></a><span data-ttu-id="669d9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="669d9-134">Response</span></span>
<span data-ttu-id="669d9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="669d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-createdobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
