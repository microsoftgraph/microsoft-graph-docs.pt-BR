---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c5327c246c3a1dc58b0b1431fdff330cf7b6a732
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526309"
---
# <a name="list-registeredusers"></a><span data-ttu-id="20cca-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="20cca-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20cca-104">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="20cca-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="20cca-105">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="20cca-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="20cca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20cca-106">Permissions</span></span>
<span data-ttu-id="20cca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20cca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20cca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20cca-109">Permission type</span></span>      | <span data-ttu-id="20cca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20cca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20cca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20cca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20cca-112">Directory.Read.All ou Directory.ReadWrite.All ou Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20cca-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20cca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20cca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20cca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20cca-114">Not supported.</span></span> |
|<span data-ttu-id="20cca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20cca-115">Application</span></span> | <span data-ttu-id="20cca-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20cca-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20cca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20cca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="20cca-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="20cca-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="20cca-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20cca-119">Optional query parameters</span></span>
<span data-ttu-id="20cca-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20cca-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="20cca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20cca-121">Request headers</span></span>
| <span data-ttu-id="20cca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="20cca-122">Name</span></span>       | <span data-ttu-id="20cca-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="20cca-123">Type</span></span> | <span data-ttu-id="20cca-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="20cca-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20cca-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="20cca-125">Authorization</span></span>  | <span data-ttu-id="20cca-126">string</span><span class="sxs-lookup"><span data-stu-id="20cca-126">string</span></span>  | <span data-ttu-id="20cca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20cca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20cca-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20cca-129">Request body</span></span>
<span data-ttu-id="20cca-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20cca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20cca-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="20cca-131">Response</span></span>

<span data-ttu-id="20cca-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20cca-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20cca-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20cca-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20cca-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20cca-134">Request</span></span>
<span data-ttu-id="20cca-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20cca-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="20cca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="20cca-136">Response</span></span>
<span data-ttu-id="20cca-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20cca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-registeredusers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
