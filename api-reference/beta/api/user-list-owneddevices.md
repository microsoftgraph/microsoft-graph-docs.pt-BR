---
title: Listar ownedDevices
description: Obtenha a lista de dispositivos de propriedade do usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c9ba8f48eb62b73408f956badb53560f3e9550b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544292"
---
# <a name="list-owneddevices"></a><span data-ttu-id="2c587-103">Listar ownedDevices</span><span class="sxs-lookup"><span data-stu-id="2c587-103">List ownedDevices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c587-104">Obtenha a lista de dispositivos de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="2c587-104">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c587-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c587-105">Permissions</span></span>
<span data-ttu-id="2c587-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c587-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c587-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c587-108">Permission type</span></span>      | <span data-ttu-id="2c587-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c587-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c587-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c587-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c587-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c587-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c587-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c587-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c587-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c587-113">Not supported.</span></span>    |
|<span data-ttu-id="2c587-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c587-114">Application</span></span> | <span data-ttu-id="2c587-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c587-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c587-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c587-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2c587-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2c587-117">Optional query parameters</span></span>
<span data-ttu-id="2c587-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c587-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2c587-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c587-119">Request headers</span></span>
| <span data-ttu-id="2c587-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c587-120">Header</span></span>       | <span data-ttu-id="2c587-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2c587-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c587-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c587-122">Authorization</span></span>  | <span data-ttu-id="2c587-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c587-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c587-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c587-125">Accept</span></span>  | <span data-ttu-id="2c587-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2c587-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c587-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c587-127">Request body</span></span>
<span data-ttu-id="2c587-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c587-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c587-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c587-129">Response</span></span>

<span data-ttu-id="2c587-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c587-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c587-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c587-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c587-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c587-132">Request</span></span>
<span data-ttu-id="2c587-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c587-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/ownedDevices
```
##### <a name="response"></a><span data-ttu-id="2c587-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c587-134">Response</span></span>
<span data-ttu-id="2c587-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c587-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-owneddevices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
