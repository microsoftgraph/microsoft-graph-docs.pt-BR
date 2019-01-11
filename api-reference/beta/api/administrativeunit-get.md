---
title: Obter administrativeUnit
description: Recupere as propriedades e relacionamentos de um objeto administrativeUnit.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 12c7931d0ff2e26a5298cf3fecf92a7bee55e9ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849291"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="7091c-103">Obter administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="7091c-103">Get administrativeUnit</span></span>

> <span data-ttu-id="7091c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7091c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7091c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7091c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7091c-106">Recupere as propriedades e relacionamentos de um objeto [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="7091c-106">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="7091c-107">Desde que o recurso de **administrativeUnit** oferece suporte às [extensões](/graph/extensibility-overview), você também pode usar o `GET` operação obter dados de extensão e propriedades personalizadas em uma instância de **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="7091c-107">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="7091c-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="7091c-108">Permissions</span></span>
<span data-ttu-id="7091c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7091c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7091c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7091c-111">Permission type</span></span>      | <span data-ttu-id="7091c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7091c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7091c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7091c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7091c-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7091c-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7091c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7091c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7091c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7091c-116">Not supported.</span></span>    |
|<span data-ttu-id="7091c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7091c-117">Application</span></span> | <span data-ttu-id="7091c-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7091c-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7091c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7091c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7091c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7091c-120">Optional query parameters</span></span>
<span data-ttu-id="7091c-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7091c-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7091c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7091c-122">Request headers</span></span>
| <span data-ttu-id="7091c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7091c-123">Name</span></span>      |<span data-ttu-id="7091c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7091c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7091c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="7091c-125">Authorization</span></span>  | <span data-ttu-id="7091c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7091c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7091c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7091c-128">Request body</span></span>
<span data-ttu-id="7091c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7091c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7091c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7091c-130">Response</span></span>

<span data-ttu-id="7091c-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [administrativeUnit](../resources/administrativeunit.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7091c-131">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7091c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7091c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7091c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7091c-133">Request</span></span>
<span data-ttu-id="7091c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7091c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="7091c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7091c-135">Response</span></span>
<span data-ttu-id="7091c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7091c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="7091c-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="7091c-139">See also</span></span>

- [<span data-ttu-id="7091c-140">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="7091c-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7091c-141">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="7091c-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
