---
title: 'Aplicativo: calcular'
description: Recalcula todas as pastas de trabalho abertas no Excel no momento.
localization_priority: Normal
ms.openlocfilehash: 3d80fc89c002d7c89fcc5d68920895b9b1fe1c4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818330"
---
# <a name="application-calculate"></a><span data-ttu-id="001ce-103">Aplicativo: calcular</span><span class="sxs-lookup"><span data-stu-id="001ce-103">Application: calculate</span></span>

> <span data-ttu-id="001ce-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="001ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="001ce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="001ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="001ce-106">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="001ce-106">Recalculate all currently opened workbooks in Excel.</span></span>
## <a name="permissions"></a><span data-ttu-id="001ce-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="001ce-107">Permissions</span></span>
<span data-ttu-id="001ce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="001ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="001ce-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="001ce-110">Permission type</span></span>      | <span data-ttu-id="001ce-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="001ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="001ce-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="001ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="001ce-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="001ce-113">Not supported.</span></span>    |
|<span data-ttu-id="001ce-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="001ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="001ce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="001ce-115">Not supported.</span></span>    |
|<span data-ttu-id="001ce-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="001ce-116">Application</span></span> | <span data-ttu-id="001ce-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="001ce-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="001ce-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="001ce-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/application/calculate

```
## <a name="request-headers"></a><span data-ttu-id="001ce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="001ce-119">Request headers</span></span>
| <span data-ttu-id="001ce-120">Nome</span><span class="sxs-lookup"><span data-stu-id="001ce-120">Name</span></span>       | <span data-ttu-id="001ce-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="001ce-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="001ce-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="001ce-122">Authorization</span></span>  | <span data-ttu-id="001ce-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="001ce-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="001ce-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="001ce-125">Request body</span></span>
<span data-ttu-id="001ce-126">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="001ce-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="001ce-127">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="001ce-127">Parameter</span></span>    | <span data-ttu-id="001ce-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="001ce-128">Type</span></span>   |<span data-ttu-id="001ce-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="001ce-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="001ce-130">calculationType</span><span class="sxs-lookup"><span data-stu-id="001ce-130">calculationType</span></span>|<span data-ttu-id="001ce-131">string</span><span class="sxs-lookup"><span data-stu-id="001ce-131">string</span></span>|<span data-ttu-id="001ce-132">Especifica o tipo de cálculo a ser usado.</span><span class="sxs-lookup"><span data-stu-id="001ce-132">Specifies the calculation type to use.</span></span>  <span data-ttu-id="001ce-133">Os valores possíveis são: `Recalculate`, `Full`, `FullRebuild`.</span><span class="sxs-lookup"><span data-stu-id="001ce-133">Possible values are: `Recalculate`, `Full`, `FullRebuild`.</span></span>|

## <a name="response"></a><span data-ttu-id="001ce-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="001ce-134">Response</span></span>

<span data-ttu-id="001ce-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="001ce-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="001ce-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="001ce-137">Example</span></span>
<span data-ttu-id="001ce-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="001ce-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="001ce-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="001ce-139">Request</span></span>
<span data-ttu-id="001ce-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="001ce-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "application_calculate"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application/calculate
Content-type: application/json
Content-length: 48

{
  "calculationType": "calculationType-value"
}
```

##### <a name="response"></a><span data-ttu-id="001ce-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="001ce-141">Response</span></span>
<span data-ttu-id="001ce-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="001ce-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Application: calculate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
