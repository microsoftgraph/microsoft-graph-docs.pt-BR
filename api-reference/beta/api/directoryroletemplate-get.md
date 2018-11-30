---
title: Obter directoryRoleTemplate
description: Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.
ms.openlocfilehash: 007b290d1bf0b33f47977d3c53a5a2ae66700136
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033641"
---
# <a name="get-directoryroletemplate"></a><span data-ttu-id="5b6f8-103">Obter directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="5b6f8-103">Get directoryRoleTemplate</span></span>

> <span data-ttu-id="5b6f8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b6f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b6f8-106">Recupera as propriedades e os relacionamentos do objeto directoryroletemplate.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-106">Retrieve the properties and relationships of a directoryroletemplate object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5b6f8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5b6f8-107">Permissions</span></span>
<span data-ttu-id="5b6f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b6f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b6f8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b6f8-110">Permission type</span></span>      | <span data-ttu-id="5b6f8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b6f8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b6f8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b6f8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b6f8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5b6f8-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b6f8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b6f8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b6f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-115">Not supported.</span></span>    |
|<span data-ttu-id="5b6f8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b6f8-116">Application</span></span> | <span data-ttu-id="5b6f8-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b6f8-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b6f8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b6f8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b6f8-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5b6f8-119">Optional query parameters</span></span>
<span data-ttu-id="5b6f8-120">Esse método **não** tem suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="5b6f8-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b6f8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6f8-121">Request headers</span></span>
| <span data-ttu-id="5b6f8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5b6f8-122">Name</span></span>       | <span data-ttu-id="5b6f8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b6f8-123">Type</span></span> | <span data-ttu-id="5b6f8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b6f8-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5b6f8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b6f8-125">Authorization</span></span>  | <span data-ttu-id="5b6f8-126">string</span><span class="sxs-lookup"><span data-stu-id="5b6f8-126">string</span></span>  | <span data-ttu-id="5b6f8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b6f8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6f8-129">Request body</span></span>
<span data-ttu-id="5b6f8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b6f8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6f8-131">Response</span></span>

<span data-ttu-id="5b6f8-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRoleTemplate](../resources/directoryroletemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-132">If successful, this method returns a `200 OK` response code and [directoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5b6f8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b6f8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b6f8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b6f8-134">Request</span></span>
<span data-ttu-id="5b6f8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplate"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoleTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="5b6f8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b6f8-136">Response</span></span>
<span data-ttu-id="5b6f8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b6f8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "description": "description-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
