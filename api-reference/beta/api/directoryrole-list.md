---
title: Listar directoryRoles
description: Lista as funções de diretório ativadas no locatário.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b50af15f6bce8bb6d6fdb4072df71edbf19a9cf7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956154"
---
# <a name="list-directoryroles"></a><span data-ttu-id="97bd8-103">Listar directoryRoles</span><span class="sxs-lookup"><span data-stu-id="97bd8-103">List directoryRoles</span></span>

> <span data-ttu-id="97bd8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="97bd8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97bd8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97bd8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97bd8-106">Lista as funções de diretório ativadas no locatário.</span><span class="sxs-lookup"><span data-stu-id="97bd8-106">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="97bd8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="97bd8-107">Permissions</span></span>
<span data-ttu-id="97bd8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97bd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97bd8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97bd8-110">Permission type</span></span>      | <span data-ttu-id="97bd8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97bd8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97bd8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97bd8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="97bd8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="97bd8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97bd8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97bd8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97bd8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97bd8-115">Not supported.</span></span>    |
|<span data-ttu-id="97bd8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97bd8-116">Application</span></span> | <span data-ttu-id="97bd8-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97bd8-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97bd8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97bd8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97bd8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97bd8-119">Optional query parameters</span></span>
<span data-ttu-id="97bd8-120">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="97bd8-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="97bd8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97bd8-121">Request headers</span></span>
| <span data-ttu-id="97bd8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="97bd8-122">Name</span></span>       | <span data-ttu-id="97bd8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="97bd8-123">Type</span></span> | <span data-ttu-id="97bd8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="97bd8-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97bd8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="97bd8-125">Authorization</span></span>  | <span data-ttu-id="97bd8-126">string</span><span class="sxs-lookup"><span data-stu-id="97bd8-126">string</span></span>  | <span data-ttu-id="97bd8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97bd8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97bd8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97bd8-129">Request body</span></span>
<span data-ttu-id="97bd8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97bd8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97bd8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="97bd8-131">Response</span></span>

<span data-ttu-id="97bd8-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97bd8-132">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97bd8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97bd8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97bd8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97bd8-134">Request</span></span>
<span data-ttu-id="97bd8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97bd8-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="97bd8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="97bd8-136">Response</span></span>
<span data-ttu-id="97bd8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97bd8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
