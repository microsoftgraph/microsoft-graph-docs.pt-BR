---
title: Excluir synchronizationSchema
description: Exclui o esquema personalizado e redefine o esquema para a configuração padrão. Se o esquema for excluído no contexto do modelo, ele redefine o esquema para o padrão de um associado do modelo `factoryTag`.
localization_priority: Normal
ms.openlocfilehash: cb4c6295fe962ea9570da19b9b6ee8190b2024f5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526988"
---
# <a name="delete-synchronizationschema"></a><span data-ttu-id="81b22-104">Excluir synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="81b22-104">Delete synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81b22-105">Exclui o esquema personalizado e redefine o esquema para a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="81b22-105">Deletes the customized schema and resets the schema to the default configuration.</span></span> <span data-ttu-id="81b22-106">Se o esquema for excluído no contexto do modelo, ele redefine o esquema para o padrão de um associado do modelo `factoryTag`.</span><span class="sxs-lookup"><span data-stu-id="81b22-106">If the schema is deleted in the context of the template, it resets the schema to the default one associated with the template's `factoryTag`.</span></span>

## <a name="permissions"></a><span data-ttu-id="81b22-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="81b22-107">Permissions</span></span>
<span data-ttu-id="81b22-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81b22-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81b22-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81b22-110">Permission type</span></span>                        | <span data-ttu-id="81b22-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81b22-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="81b22-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81b22-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="81b22-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81b22-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="81b22-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81b22-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="81b22-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81b22-115">Not supported.</span></span>|
|<span data-ttu-id="81b22-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81b22-116">Application</span></span>                            |<span data-ttu-id="81b22-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81b22-117">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="81b22-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81b22-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
DELETE /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="81b22-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81b22-119">Request headers</span></span>

| <span data-ttu-id="81b22-120">Nome</span><span class="sxs-lookup"><span data-stu-id="81b22-120">Name</span></span>           | <span data-ttu-id="81b22-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="81b22-121">Type</span></span>    | <span data-ttu-id="81b22-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="81b22-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="81b22-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="81b22-123">Authorization</span></span>  | <span data-ttu-id="81b22-124">string</span><span class="sxs-lookup"><span data-stu-id="81b22-124">string</span></span>  | <span data-ttu-id="81b22-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81b22-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81b22-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81b22-127">Request body</span></span>

<span data-ttu-id="81b22-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81b22-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81b22-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b22-129">Response</span></span>

<span data-ttu-id="81b22-130">Se tiver êxito, este método retornará um código de resposta `201 No Content`.</span><span class="sxs-lookup"><span data-stu-id="81b22-130">If successful, this method returns a `201 No Content` response code.</span></span> <span data-ttu-id="81b22-131">Ele não retornará nada no corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81b22-131">It does not return anything in response body.</span></span>

## <a name="example"></a><span data-ttu-id="81b22-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81b22-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="81b22-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81b22-133">Request</span></span>
<span data-ttu-id="81b22-134">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="81b22-134">The following is an example of a request.</span></span>

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="81b22-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="81b22-135">Response</span></span>
<span data-ttu-id="81b22-136">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="81b22-136">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
