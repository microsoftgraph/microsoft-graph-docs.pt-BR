---
title: Lista privilegedRoles
description: Recupere uma lista de objetos privilegedRole.
localization_priority: Normal
ms.openlocfilehash: d954cedbaf4b164fe0649a3565ea0212d148c322
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518076"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="71dea-103">Lista privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="71dea-103">List privilegedRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71dea-104">Recupere uma lista de objetos [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="71dea-104">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="71dea-105">Para filtrar os resultados da consulta, use o OData standard ``$filter`` expressões nos URIs.</span><span class="sxs-lookup"><span data-stu-id="71dea-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="71dea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71dea-106">Permissions</span></span>
<span data-ttu-id="71dea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="71dea-109">O solicitante precisa ter uma das seguintes funções: _Leitor de segurança_, _Administrador Global_, _Administrador de segurança_ou _Administrador com privilégios de função_.</span><span class="sxs-lookup"><span data-stu-id="71dea-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="71dea-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71dea-110">Permission type</span></span>      | <span data-ttu-id="71dea-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71dea-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71dea-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71dea-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71dea-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71dea-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71dea-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71dea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71dea-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71dea-115">Not supported.</span></span>    |
|<span data-ttu-id="71dea-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71dea-116">Application</span></span> | <span data-ttu-id="71dea-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71dea-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71dea-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71dea-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71dea-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71dea-119">Optional query parameters</span></span>
<span data-ttu-id="71dea-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71dea-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71dea-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71dea-121">Request headers</span></span>
| <span data-ttu-id="71dea-122">Nome</span><span class="sxs-lookup"><span data-stu-id="71dea-122">Name</span></span>      |<span data-ttu-id="71dea-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="71dea-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71dea-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="71dea-124">Authorization</span></span>  | <span data-ttu-id="71dea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71dea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71dea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71dea-127">Request body</span></span>
<span data-ttu-id="71dea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71dea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71dea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="71dea-129">Response</span></span>

<span data-ttu-id="71dea-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71dea-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="71dea-131">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="71dea-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="71dea-132">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="71dea-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="71dea-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71dea-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71dea-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71dea-134">Request</span></span>
<span data-ttu-id="71dea-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71dea-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
##### <a name="response"></a><span data-ttu-id="71dea-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="71dea-136">Response</span></span>
<span data-ttu-id="71dea-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71dea-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
