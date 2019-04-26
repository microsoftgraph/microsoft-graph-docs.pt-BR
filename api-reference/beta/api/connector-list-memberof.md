---
title: Listar memberOf
description: Recupere o MemberGroup do qual o conector é membro.
localization_priority: Normal
ms.openlocfilehash: 19d6e8c45751f5c257c00381c90e77b7bff0bb19
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327475"
---
# <a name="list-memberof"></a><span data-ttu-id="17cf8-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="17cf8-103">List memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17cf8-104">Recupere o MemberGroup do qual o conector é membro.</span><span class="sxs-lookup"><span data-stu-id="17cf8-104">Retrieve the connectorgroup the connector is a member of.</span></span>
## <a name="permissions"></a><span data-ttu-id="17cf8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="17cf8-105">Permissions</span></span>
<span data-ttu-id="17cf8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17cf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17cf8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17cf8-108">Permission type</span></span>      | <span data-ttu-id="17cf8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17cf8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17cf8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17cf8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17cf8-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17cf8-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17cf8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17cf8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17cf8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17cf8-113">Not supported.</span></span>    |
|<span data-ttu-id="17cf8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17cf8-114">Application</span></span> | <span data-ttu-id="17cf8-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17cf8-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17cf8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17cf8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17cf8-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17cf8-117">Optional query parameters</span></span>
<span data-ttu-id="17cf8-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="17cf8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17cf8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17cf8-119">Request headers</span></span>
| <span data-ttu-id="17cf8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="17cf8-120">Name</span></span>      |<span data-ttu-id="17cf8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="17cf8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17cf8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="17cf8-122">Authorization</span></span>  | <span data-ttu-id="17cf8-123">Portador.</span><span class="sxs-lookup"><span data-stu-id="17cf8-123">Bearer.</span></span> <span data-ttu-id="17cf8-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="17cf8-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="17cf8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17cf8-125">Request body</span></span>
<span data-ttu-id="17cf8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17cf8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17cf8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="17cf8-127">Response</span></span>

<span data-ttu-id="17cf8-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos do grupo de [conectores](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17cf8-128">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17cf8-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17cf8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17cf8-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17cf8-130">Request</span></span>
<span data-ttu-id="17cf8-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17cf8-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
```
##### <a name="response"></a><span data-ttu-id="17cf8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="17cf8-132">Response</span></span>
<span data-ttu-id="17cf8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17cf8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
