---
title: Lista privilegedRoles
description: Recupere uma lista de objetos privilegedRole.
ms.openlocfilehash: 6800096f36e1fb8237216cf9ea708b3b20ff21ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035932"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="54875-103">Lista privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="54875-103">List privilegedRoles</span></span>

> <span data-ttu-id="54875-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="54875-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54875-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="54875-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54875-106">Recupere uma lista de objetos [privilegedRole](../resources/privilegedrole.md) .</span><span class="sxs-lookup"><span data-stu-id="54875-106">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="54875-107">Para filtrar os resultados da consulta, use o OData standard ``$filter`` expressões nos URIs.</span><span class="sxs-lookup"><span data-stu-id="54875-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="54875-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="54875-108">Permissions</span></span>
<span data-ttu-id="54875-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54875-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="54875-111">O solicitante precisa ter uma das seguintes funções: _Leitor de segurança_, _Administrador Global_, _Administrador de segurança_ou _Administrador com privilégios de função_.</span><span class="sxs-lookup"><span data-stu-id="54875-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="54875-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54875-112">Permission type</span></span>      | <span data-ttu-id="54875-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54875-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54875-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54875-114">Delegated (work or school account)</span></span> | <span data-ttu-id="54875-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="54875-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="54875-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54875-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54875-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54875-117">Not supported.</span></span>    |
|<span data-ttu-id="54875-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54875-118">Application</span></span> | <span data-ttu-id="54875-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54875-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54875-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54875-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54875-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54875-121">Optional query parameters</span></span>
<span data-ttu-id="54875-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="54875-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54875-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54875-123">Request headers</span></span>
| <span data-ttu-id="54875-124">Nome</span><span class="sxs-lookup"><span data-stu-id="54875-124">Name</span></span>      |<span data-ttu-id="54875-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="54875-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54875-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="54875-126">Authorization</span></span>  | <span data-ttu-id="54875-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54875-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54875-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54875-129">Request body</span></span>
<span data-ttu-id="54875-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54875-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54875-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="54875-131">Response</span></span>

<span data-ttu-id="54875-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [privilegedRole](../resources/privilegedrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54875-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="54875-133">Observe que o inquilino deve ser registrado no PIM.</span><span class="sxs-lookup"><span data-stu-id="54875-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="54875-134">Caso contrário, será retornado o código de status HTTP 403-Proibido.</span><span class="sxs-lookup"><span data-stu-id="54875-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="54875-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54875-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54875-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54875-136">Request</span></span>
<span data-ttu-id="54875-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="54875-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
##### <a name="response"></a><span data-ttu-id="54875-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="54875-138">Response</span></span>
<span data-ttu-id="54875-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54875-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->