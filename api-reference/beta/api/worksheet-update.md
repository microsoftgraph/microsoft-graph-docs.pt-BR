---
title: Atualizar planilha
description: Atualize as propriedades do objeto de planilha.
ms.openlocfilehash: 16db37919009dbd935bcd8959111f888ffa97d2e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036941"
---
# <a name="update-worksheet"></a><span data-ttu-id="6e9a6-103">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="6e9a6-103">Update worksheet</span></span>

> <span data-ttu-id="6e9a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e9a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e9a6-106">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-106">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e9a6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e9a6-107">Permissions</span></span>
<span data-ttu-id="6e9a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e9a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e9a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e9a6-110">Permission type</span></span>      | <span data-ttu-id="6e9a6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e9a6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e9a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e9a6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6e9a6-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e9a6-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6e9a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e9a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e9a6-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e9a6-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="6e9a6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e9a6-116">Application</span></span> | <span data-ttu-id="6e9a6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e9a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e9a6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="6e9a6-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6e9a6-119">Optional request headers</span></span>
| <span data-ttu-id="6e9a6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6e9a6-120">Name</span></span>       | <span data-ttu-id="6e9a6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e9a6-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6e9a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e9a6-122">Authorization</span></span>  | <span data-ttu-id="6e9a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e9a6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6e9a6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6e9a6-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e9a6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e9a6-128">Request body</span></span>
<span data-ttu-id="6e9a6-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6e9a6-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e9a6-132">Property</span></span>     | <span data-ttu-id="6e9a6-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e9a6-133">Type</span></span>   |<span data-ttu-id="6e9a6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e9a6-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e9a6-135">name</span><span class="sxs-lookup"><span data-stu-id="6e9a6-135">name</span></span>|<span data-ttu-id="6e9a6-136">string</span><span class="sxs-lookup"><span data-stu-id="6e9a6-136">string</span></span>|<span data-ttu-id="6e9a6-137">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-137">The display name of the worksheet.</span></span>|
|<span data-ttu-id="6e9a6-138">position</span><span class="sxs-lookup"><span data-stu-id="6e9a6-138">position</span></span>|<span data-ttu-id="6e9a6-139">inteiro</span><span class="sxs-lookup"><span data-stu-id="6e9a6-139">int</span></span>|<span data-ttu-id="6e9a6-140">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-140">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="6e9a6-141">visibilidade</span><span class="sxs-lookup"><span data-stu-id="6e9a6-141">visibility</span></span>|<span data-ttu-id="6e9a6-142">string</span><span class="sxs-lookup"><span data-stu-id="6e9a6-142">string</span></span>|<span data-ttu-id="6e9a6-p106">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-p106">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="6e9a6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e9a6-145">Response</span></span>

<span data-ttu-id="6e9a6-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Worksheet](../resources/worksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-146">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e9a6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e9a6-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e9a6-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e9a6-148">Request</span></span>
<span data-ttu-id="6e9a6-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="6e9a6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e9a6-150">Response</span></span>
<span data-ttu-id="6e9a6-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e9a6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->