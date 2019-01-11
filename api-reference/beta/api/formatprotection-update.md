---
title: Atualizar formatprotection
description: Atualiza as propriedades do objeto formatprotection.
localization_priority: Normal
ms.openlocfilehash: f94713c3bdc729c02dcedae0905013be81f1687d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837783"
---
# <a name="update-formatprotection"></a><span data-ttu-id="4af28-103">Atualizar formatprotection</span><span class="sxs-lookup"><span data-stu-id="4af28-103">Update formatprotection</span></span>

> <span data-ttu-id="4af28-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4af28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4af28-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4af28-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4af28-106">Atualiza as propriedades do objeto formatprotection.</span><span class="sxs-lookup"><span data-stu-id="4af28-106">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4af28-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4af28-107">Permissions</span></span>
<span data-ttu-id="4af28-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4af28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4af28-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4af28-110">Permission type</span></span>      | <span data-ttu-id="4af28-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4af28-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4af28-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4af28-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4af28-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4af28-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4af28-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4af28-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4af28-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4af28-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4af28-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4af28-116">Application</span></span> | <span data-ttu-id="4af28-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4af28-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4af28-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4af28-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="4af28-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4af28-119">Optional request headers</span></span>
| <span data-ttu-id="4af28-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4af28-120">Name</span></span>       | <span data-ttu-id="4af28-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4af28-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4af28-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4af28-122">Authorization</span></span>  | <span data-ttu-id="4af28-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4af28-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4af28-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4af28-125">Request body</span></span>
<span data-ttu-id="4af28-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4af28-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4af28-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4af28-129">Property</span></span>     | <span data-ttu-id="4af28-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4af28-130">Type</span></span>   |<span data-ttu-id="4af28-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4af28-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4af28-132">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="4af28-132">formulaHidden</span></span>|<span data-ttu-id="4af28-133">booliano</span><span class="sxs-lookup"><span data-stu-id="4af28-133">boolean</span></span>|<span data-ttu-id="4af28-p105">Indica se o Excel ocultará a fórmula para as células no intervalo. Um valor nulo indica que o intervalo inteiro não tem configuração uniforme de fórmula oculta.</span><span class="sxs-lookup"><span data-stu-id="4af28-p105">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="4af28-136">locked</span><span class="sxs-lookup"><span data-stu-id="4af28-136">locked</span></span>|<span data-ttu-id="4af28-137">booliano</span><span class="sxs-lookup"><span data-stu-id="4af28-137">boolean</span></span>|<span data-ttu-id="4af28-p106">Indica se o Excel bloqueia as células no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de bloqueio uniforme.</span><span class="sxs-lookup"><span data-stu-id="4af28-p106">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="4af28-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4af28-140">Response</span></span>

<span data-ttu-id="4af28-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [FormatProtection](../resources/formatprotection.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4af28-141">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4af28-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4af28-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4af28-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4af28-143">Request</span></span>
<span data-ttu-id="4af28-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4af28-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="4af28-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4af28-145">Response</span></span>
<span data-ttu-id="4af28-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4af28-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
