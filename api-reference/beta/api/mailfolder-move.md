---
title: 'mailFolder: move'
description: Mova uma mailFolder e seu conteúdo para outra mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 836c91ee2bfd234c5c831511d1be45800be8660a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540699"
---
# <a name="mailfolder-move"></a><span data-ttu-id="5a83c-103">mailFolder: move</span><span class="sxs-lookup"><span data-stu-id="5a83c-103">mailFolder: move</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a83c-104">Mova uma mailFolder e seu conteúdo para outra mailFolder.</span><span class="sxs-lookup"><span data-stu-id="5a83c-104">Move a mailfolder and its contents to another mailfolder.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a83c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a83c-105">Permissions</span></span>

<span data-ttu-id="5a83c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a83c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a83c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a83c-108">Permission type</span></span> | <span data-ttu-id="5a83c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a83c-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="5a83c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a83c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5a83c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a83c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5a83c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a83c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a83c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a83c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5a83c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a83c-114">Application</span></span> | <span data-ttu-id="5a83c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a83c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a83c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a83c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/mailFolders/{id}/move
POST /users/{id | userPrincipalName}/mailFolders/{id}/move
```

## <a name="request-headers"></a><span data-ttu-id="5a83c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a83c-117">Request headers</span></span>

| <span data-ttu-id="5a83c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a83c-118">Header</span></span> | <span data-ttu-id="5a83c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="5a83c-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="5a83c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a83c-120">Authorization</span></span> | <span data-ttu-id="5a83c-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="5a83c-121"></span></span> <span data-ttu-id="5a83c-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a83c-122">Required.</span></span> |
| <span data-ttu-id="5a83c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a83c-123">Content-Type</span></span> | <span data-ttu-id="5a83c-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="5a83c-124"></span></span> <span data-ttu-id="5a83c-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a83c-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a83c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a83c-126">Request body</span></span>

<span data-ttu-id="5a83c-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a83c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a83c-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5a83c-128">Parameter</span></span> | <span data-ttu-id="5a83c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a83c-129">Type</span></span> | <span data-ttu-id="5a83c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a83c-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="5a83c-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="5a83c-131">destinationId</span></span>|<span data-ttu-id="5a83c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a83c-132">String</span></span>|<span data-ttu-id="5a83c-133">A ID da pasta ou um nome de pasta conhecido.</span><span class="sxs-lookup"><span data-stu-id="5a83c-133">The folder ID, or a well-known folder name.</span></span> <span data-ttu-id="5a83c-134">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5a83c-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="5a83c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a83c-135">Response</span></span>

<span data-ttu-id="5a83c-136">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a83c-136">If successful, this method returns `200 OK` response code and a [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a83c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a83c-137">Example</span></span>

<span data-ttu-id="5a83c-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5a83c-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5a83c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a83c-139">Request</span></span>

<span data-ttu-id="5a83c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a83c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "mailfolder_move"
}-->

```http
POST https://graph.microsoft.com/beta/me/mailFolders/{id}/move
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```

##### <a name="response"></a><span data-ttu-id="5a83c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a83c-141">Response</span></span>

<span data-ttu-id="5a83c-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a83c-142">Here is an example of the response.</span></span>

> <span data-ttu-id="5a83c-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5a83c-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5a83c-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a83c-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder: move",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-move.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
