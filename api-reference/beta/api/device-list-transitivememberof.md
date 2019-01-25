---
title: Listar grupos transitivos do dispositivo
description: Obtenha os grupos que o dispositivo é um membro de. Essa solicitação API é transitiva e também retornará todos os grupos que o dispositivo é um membro aninhado do.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 69cd4e4be3f02d3609bc9f0af2f094533c67dba7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528162"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="bcb69-104">Listar grupos transitivos do dispositivo</span><span class="sxs-lookup"><span data-stu-id="bcb69-104">List device transitive groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcb69-105">Obtenha os grupos que o dispositivo é um membro de.</span><span class="sxs-lookup"><span data-stu-id="bcb69-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="bcb69-106">Essa solicitação API é transitiva e também retornará todos os grupos que o dispositivo é um membro aninhado do.</span><span class="sxs-lookup"><span data-stu-id="bcb69-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcb69-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bcb69-107">Permissions</span></span>

<span data-ttu-id="bcb69-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcb69-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcb69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcb69-110">Permission type</span></span>      | <span data-ttu-id="bcb69-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcb69-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcb69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcb69-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bcb69-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bcb69-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bcb69-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcb69-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcb69-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcb69-115">Not supported.</span></span>    |
|<span data-ttu-id="bcb69-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcb69-116">Application</span></span> | <span data-ttu-id="bcb69-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcb69-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcb69-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcb69-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcb69-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bcb69-119">Optional query parameters</span></span>

<span data-ttu-id="bcb69-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bcb69-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bcb69-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcb69-121">Request headers</span></span>

| <span data-ttu-id="bcb69-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcb69-122">Header</span></span>       | <span data-ttu-id="bcb69-123">Valor</span><span class="sxs-lookup"><span data-stu-id="bcb69-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bcb69-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcb69-124">Authorization</span></span>  | <span data-ttu-id="bcb69-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcb69-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bcb69-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bcb69-127">Accept</span></span>  | <span data-ttu-id="bcb69-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bcb69-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcb69-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcb69-129">Request body</span></span>

<span data-ttu-id="bcb69-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bcb69-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcb69-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcb69-131">Response</span></span>

<span data-ttu-id="bcb69-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcb69-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcb69-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcb69-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcb69-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcb69-134">Request</span></span>

<span data-ttu-id="bcb69-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcb69-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="bcb69-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcb69-136">Response</span></span>

<span data-ttu-id="bcb69-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcb69-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
