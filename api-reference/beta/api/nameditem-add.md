---
title: Adicionar Item nomeado
description: Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.
localization_priority: Normal
ms.openlocfilehash: 57ae84505327f2afbe2936b2671b655e76a85bd4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836698"
---
# <a name="add-named-item"></a><span data-ttu-id="dfc36-103">Adicionar Item nomeado</span><span class="sxs-lookup"><span data-stu-id="dfc36-103">Add Named Item</span></span>

> <span data-ttu-id="dfc36-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dfc36-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfc36-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dfc36-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfc36-106">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="dfc36-106">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfc36-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfc36-107">Permissions</span></span>
<span data-ttu-id="dfc36-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfc36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfc36-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfc36-110">Permission type</span></span>      | <span data-ttu-id="dfc36-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfc36-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfc36-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfc36-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dfc36-113">Files.ReadWrite, Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc36-113">Files.ReadWrite, Sites.Read.All</span></span>    |
|<span data-ttu-id="dfc36-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfc36-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfc36-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dfc36-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="dfc36-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfc36-116">Application</span></span> | <span data-ttu-id="dfc36-117">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc36-117">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfc36-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc36-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/add
POST /workbook/worksheets({id|name})/names/add

```
## <a name="request-headers"></a><span data-ttu-id="dfc36-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc36-119">Request headers</span></span>
| <span data-ttu-id="dfc36-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dfc36-120">Name</span></span>       | <span data-ttu-id="dfc36-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfc36-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dfc36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfc36-122">Authorization</span></span>  | <span data-ttu-id="dfc36-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfc36-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfc36-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="dfc36-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="dfc36-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="dfc36-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfc36-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc36-128">Request body</span></span>
<span data-ttu-id="dfc36-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfc36-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dfc36-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dfc36-130">Parameter</span></span>    | <span data-ttu-id="dfc36-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfc36-131">Type</span></span>   |<span data-ttu-id="dfc36-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfc36-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dfc36-133">name</span><span class="sxs-lookup"><span data-stu-id="dfc36-133">name</span></span>|<span data-ttu-id="dfc36-134">string</span><span class="sxs-lookup"><span data-stu-id="dfc36-134">string</span></span>|<span data-ttu-id="dfc36-135">O nome do item nomeado.</span><span class="sxs-lookup"><span data-stu-id="dfc36-135">The name of the named item.</span></span>|
|<span data-ttu-id="dfc36-136">reference</span><span class="sxs-lookup"><span data-stu-id="dfc36-136">reference</span></span>|<span data-ttu-id="dfc36-137">string</span><span class="sxs-lookup"><span data-stu-id="dfc36-137">string</span></span>|<span data-ttu-id="dfc36-138">A fórmula ou o intervalo ao qual o nome fará referência.</span><span class="sxs-lookup"><span data-stu-id="dfc36-138">The formula or the range that the name will refer to.</span></span>|
|<span data-ttu-id="dfc36-139">comentário</span><span class="sxs-lookup"><span data-stu-id="dfc36-139">comment</span></span>|<span data-ttu-id="dfc36-140">string</span><span class="sxs-lookup"><span data-stu-id="dfc36-140">string</span></span>|<span data-ttu-id="dfc36-141">O comentário associado ao item nomeado</span><span class="sxs-lookup"><span data-stu-id="dfc36-141">The comment associated with the named item</span></span>|

## <a name="response"></a><span data-ttu-id="dfc36-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc36-142">Response</span></span>

<span data-ttu-id="dfc36-143">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [NamedItem](../resources/nameditem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfc36-143">If successful, this method returns `200 OK` response code and [NamedItem](../resources/nameditem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfc36-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfc36-144">Example</span></span>
<span data-ttu-id="dfc36-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dfc36-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="dfc36-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfc36-146">Request</span></span>
<span data-ttu-id="dfc36-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfc36-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "NamedItemcollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names/add
Content-type: application/json
Content-length: 54

{
  "name": "test5",
  "reference": "=Sheet1!$F$15:$N$27",
  "comment": "Comment for the named item"
}


```

##### <a name="response"></a><span data-ttu-id="dfc36-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfc36-148">Response</span></span>
<span data-ttu-id="dfc36-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfc36-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookNamedItem",
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "@odata.id": "/users('ca41eb6e-5828-486b-ab52-c3bd1f7a4047')/drive/root/workbook/names(%27test5%27)",
    "comment": "Comment for the named item",
    "name": "test5",
    "scope": "Workbook",
    "type": "Range",
    "value": "Sheet1!$F$15:$N$27",
    "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItemCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
