---
title: Remover proprietário
description: Use esta API para remover um proprietário de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação owners.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 761849207983157a770c6c9cd5bea90a6c1b14ef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503047"
---
# <a name="remove-owner"></a><span data-ttu-id="892f0-103">Remover proprietário</span><span class="sxs-lookup"><span data-stu-id="892f0-103">Remove owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="892f0-104">Use esta API para remover um proprietário de um grupo do Office 365, de um grupo de segurança ou de um grupo de segurança habilitado para email através da propriedade de navegação owners.</span><span class="sxs-lookup"><span data-stu-id="892f0-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="892f0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="892f0-105">Permissions</span></span>
<span data-ttu-id="892f0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="892f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="892f0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="892f0-108">Permission type</span></span>      | <span data-ttu-id="892f0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="892f0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="892f0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="892f0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="892f0-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="892f0-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="892f0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="892f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="892f0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="892f0-113">Not supported.</span></span>    |
|<span data-ttu-id="892f0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="892f0-114">Application</span></span> | <span data-ttu-id="892f0-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="892f0-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="892f0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="892f0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="892f0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="892f0-117">Request headers</span></span>
| <span data-ttu-id="892f0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="892f0-118">Name</span></span>       | <span data-ttu-id="892f0-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="892f0-119">Type</span></span> | <span data-ttu-id="892f0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="892f0-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="892f0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="892f0-121">Authorization</span></span>  | <span data-ttu-id="892f0-122">string</span><span class="sxs-lookup"><span data-stu-id="892f0-122">string</span></span>  | <span data-ttu-id="892f0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="892f0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="892f0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="892f0-125">Request body</span></span>
<span data-ttu-id="892f0-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="892f0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="892f0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="892f0-127">Response</span></span>
<span data-ttu-id="892f0-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="892f0-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="892f0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="892f0-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="892f0-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="892f0-131">Request</span></span>
<span data-ttu-id="892f0-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="892f0-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="892f0-133">Na solicitação, especifique a `id` do objeto diretório que deseja remover após o segmento $ref.</span><span class="sxs-lookup"><span data-stu-id="892f0-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="892f0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="892f0-134">Response</span></span>
<span data-ttu-id="892f0-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="892f0-135">The following is an example of the response.</span></span>
><span data-ttu-id="892f0-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="892f0-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="892f0-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="892f0-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
