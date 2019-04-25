---
title: Listar o servicePrincipalName memberOf
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto. Essa operação não é transitiva.
localization_priority: Normal
ms.openlocfilehash: 84f82f632ef9c8f7e933d024f4d7df958415f140
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537468"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="8a21d-104">Listar o servicePrincipalName memberOf</span><span class="sxs-lookup"><span data-stu-id="8a21d-104">List servicePrincipal memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a21d-105">Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto.</span><span class="sxs-lookup"><span data-stu-id="8a21d-105">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="8a21d-106">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="8a21d-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a21d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8a21d-107">Permissions</span></span>

<span data-ttu-id="8a21d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a21d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a21d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a21d-110">Permission type</span></span>      | <span data-ttu-id="8a21d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8a21d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a21d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a21d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a21d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8a21d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8a21d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a21d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a21d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a21d-115">Not supported.</span></span>    |
|<span data-ttu-id="8a21d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8a21d-116">Application</span></span> | <span data-ttu-id="8a21d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a21d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a21d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a21d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8a21d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8a21d-119">Optional query parameters</span></span>

<span data-ttu-id="8a21d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8a21d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8a21d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a21d-121">Request headers</span></span>
| <span data-ttu-id="8a21d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8a21d-122">Name</span></span>       | <span data-ttu-id="8a21d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a21d-123">Type</span></span> | <span data-ttu-id="8a21d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a21d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8a21d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a21d-125">Authorization</span></span>  | <span data-ttu-id="8a21d-126">string</span><span class="sxs-lookup"><span data-stu-id="8a21d-126">string</span></span>  | <span data-ttu-id="8a21d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a21d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a21d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a21d-129">Request body</span></span>
<span data-ttu-id="8a21d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8a21d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a21d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a21d-131">Response</span></span>

<span data-ttu-id="8a21d-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a21d-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a21d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a21d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a21d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a21d-134">Request</span></span>

<span data-ttu-id="8a21d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a21d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="8a21d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a21d-136">Response</span></span>

<span data-ttu-id="8a21d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a21d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
