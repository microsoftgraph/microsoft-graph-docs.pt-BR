---
title: Listar registeredUsers
description: Recupera uma lista de usuários que são usuários registrados do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8e552ffe1d3bb07c365f06c4bcfcee08bdacedba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843593"
---
# <a name="list-registeredusers"></a><span data-ttu-id="0828b-103">Listar registeredUsers</span><span class="sxs-lookup"><span data-stu-id="0828b-103">List registeredUsers</span></span>

> <span data-ttu-id="0828b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0828b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0828b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0828b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0828b-106">Recupera uma lista de usuários que são usuários registrados do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0828b-106">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="0828b-107">Para dispositivos associados em nuvem e dispositivos pessoais registrados, os usuários registrados são definidos para o mesmo valor que proprietários registrados no momento do registro.</span><span class="sxs-lookup"><span data-stu-id="0828b-107">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="0828b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0828b-108">Permissions</span></span>
<span data-ttu-id="0828b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0828b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0828b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0828b-111">Permission type</span></span>      | <span data-ttu-id="0828b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0828b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0828b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0828b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0828b-114">Directory.Read.All ou Directory.ReadWrite.All ou Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0828b-114">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0828b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0828b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0828b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0828b-116">Not supported.</span></span> |
|<span data-ttu-id="0828b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0828b-117">Application</span></span> | <span data-ttu-id="0828b-118">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0828b-118">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0828b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0828b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="0828b-120">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="0828b-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="0828b-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0828b-121">Optional query parameters</span></span>
<span data-ttu-id="0828b-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0828b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0828b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0828b-123">Request headers</span></span>
| <span data-ttu-id="0828b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="0828b-124">Name</span></span>       | <span data-ttu-id="0828b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0828b-125">Type</span></span> | <span data-ttu-id="0828b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0828b-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0828b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0828b-127">Authorization</span></span>  | <span data-ttu-id="0828b-128">string</span><span class="sxs-lookup"><span data-stu-id="0828b-128">string</span></span>  | <span data-ttu-id="0828b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0828b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0828b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0828b-131">Request body</span></span>
<span data-ttu-id="0828b-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0828b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0828b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0828b-133">Response</span></span>

<span data-ttu-id="0828b-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0828b-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0828b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0828b-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0828b-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0828b-136">Request</span></span>
<span data-ttu-id="0828b-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0828b-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="0828b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0828b-138">Response</span></span>
<span data-ttu-id="0828b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0828b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
