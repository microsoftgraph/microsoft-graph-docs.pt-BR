---
title: 'workbookRange: resizedRange'
description: Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.
ms.openlocfilehash: cd2851e1b4f65162fca6e617878851b2cc8e910b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035463"
---
# <a name="workbookrange-resizedrange"></a><span data-ttu-id="2dfbc-103">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="2dfbc-103">workbookRange: resizedRange</span></span>

> <span data-ttu-id="2dfbc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2dfbc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2dfbc-106">Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-106">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="2dfbc-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2dfbc-107">Permissions</span></span>
<span data-ttu-id="2dfbc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dfbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dfbc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2dfbc-110">Permission type</span></span>      | <span data-ttu-id="2dfbc-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2dfbc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dfbc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2dfbc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2dfbc-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dfbc-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2dfbc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2dfbc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dfbc-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dfbc-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2dfbc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2dfbc-116">Application</span></span> | <span data-ttu-id="2dfbc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dfbc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2dfbc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```

## <a name="function-parameters"></a><span data-ttu-id="2dfbc-119">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="2dfbc-119">Function parameters</span></span>

| <span data-ttu-id="2dfbc-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2dfbc-120">Parameter</span></span>    | <span data-ttu-id="2dfbc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="2dfbc-121">Type</span></span>   |<span data-ttu-id="2dfbc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dfbc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dfbc-123">deltaRows</span><span class="sxs-lookup"><span data-stu-id="2dfbc-123">deltarows</span></span>|<span data-ttu-id="2dfbc-124">Int32</span><span class="sxs-lookup"><span data-stu-id="2dfbc-124">Int32</span></span>|<span data-ttu-id="2dfbc-p103">O número de linhas pelo qual expandir o canto inferior direito, referente ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo</span><span class="sxs-lookup"><span data-stu-id="2dfbc-p103">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="2dfbc-127">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="2dfbc-127">deltaColumns</span></span>|<span data-ttu-id="2dfbc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2dfbc-128">Int32</span></span>|<span data-ttu-id="2dfbc-p104">O número de colunas pelo qual expandir o canto inferior direito, em relação ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-p104">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="2dfbc-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2dfbc-131">Request headers</span></span>
| <span data-ttu-id="2dfbc-132">Nome</span><span class="sxs-lookup"><span data-stu-id="2dfbc-132">Name</span></span>       | <span data-ttu-id="2dfbc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dfbc-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2dfbc-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="2dfbc-134">Authorization</span></span>  | <span data-ttu-id="2dfbc-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2dfbc-137">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2dfbc-137">Workbook-Session-Id</span></span>  | <span data-ttu-id="2dfbc-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dfbc-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2dfbc-140">Request body</span></span>
<span data-ttu-id="2dfbc-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2dfbc-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dfbc-142">Response</span></span>

<span data-ttu-id="2dfbc-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-143">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dfbc-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2dfbc-144">Example</span></span>
<span data-ttu-id="2dfbc-145">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-145">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2dfbc-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2dfbc-146">Request</span></span>
<span data-ttu-id="2dfbc-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="2dfbc-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dfbc-148">Response</span></span>
<span data-ttu-id="2dfbc-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2dfbc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
