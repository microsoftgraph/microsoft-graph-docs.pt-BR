---
title: 'Range: Intersection'
description: Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.
author: lumine2008
ms.openlocfilehash: 0ba9767c3c7d30ee5746b5a6723fd8103c1b8533
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344552"
---
# <a name="range-intersection"></a><span data-ttu-id="b9818-103">Range: Intersection</span><span class="sxs-lookup"><span data-stu-id="b9818-103">Range: Intersection</span></span>

> <span data-ttu-id="b9818-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9818-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9818-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9818-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9818-106">Obtém o objeto de intervalo que representa a interseção retangular dos intervalos determinados.</span><span class="sxs-lookup"><span data-stu-id="b9818-106">Gets the range object that represents the rectangular intersection of the given ranges.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9818-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9818-107">Permissions</span></span>
<span data-ttu-id="b9818-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9818-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9818-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9818-110">Permission type</span></span>      | <span data-ttu-id="b9818-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9818-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9818-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9818-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9818-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9818-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9818-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9818-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9818-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b9818-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b9818-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9818-116">Application</span></span> | <span data-ttu-id="b9818-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9818-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9818-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9818-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/Intersection
GET /workbook/worksheets/{id|name}/range(address='<address>')/Intersection
GET /workbook/tables/{id|name}/columns/{id|name}/range/Intersection

```
## <a name="request-headers"></a><span data-ttu-id="b9818-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9818-119">Request headers</span></span>
| <span data-ttu-id="b9818-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b9818-120">Name</span></span>       | <span data-ttu-id="b9818-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9818-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b9818-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9818-122">Authorization</span></span>  | <span data-ttu-id="b9818-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9818-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9818-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b9818-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="b9818-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b9818-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9818-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9818-128">Request body</span></span>
<span data-ttu-id="b9818-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9818-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b9818-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b9818-130">Parameter</span></span>    | <span data-ttu-id="b9818-131">Type</span><span class="sxs-lookup"><span data-stu-id="b9818-131">Type</span></span>   |<span data-ttu-id="b9818-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9818-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b9818-133">anotherRange</span><span class="sxs-lookup"><span data-stu-id="b9818-133">anotherRange</span></span>|<span data-ttu-id="b9818-134">string</span><span class="sxs-lookup"><span data-stu-id="b9818-134">string</span></span>|<span data-ttu-id="b9818-135">O objeto de intervalo ou o endereço do intervalo que será usado para determinar a interseção de intervalos.</span><span class="sxs-lookup"><span data-stu-id="b9818-135">The range object or range address that will be used to determine the intersection of ranges.</span></span>|

## <a name="response"></a><span data-ttu-id="b9818-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9818-136">Response</span></span>

<span data-ttu-id="b9818-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [Range](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9818-137">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9818-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9818-138">Example</span></span>
<span data-ttu-id="b9818-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b9818-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b9818-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9818-140">Request</span></span>
<span data-ttu-id="b9818-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9818-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_intersection"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/Intersection
Content-type: application/json
Content-length: 42

{
  "anotherRange": "anotherRange-value"
}
```

##### <a name="response"></a><span data-ttu-id="b9818-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9818-142">Response</span></span>
<span data-ttu-id="b9818-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9818-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: Intersection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->