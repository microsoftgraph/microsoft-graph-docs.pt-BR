---
title: Atualizar contactfolder
description: Atualizar as propriedades do objeto contactfolder.
author: angelgolfer-ms
ms.openlocfilehash: 5b61758309e8489312d2f8360625d6d12566fae0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330986"
---
# <a name="update-contactfolder"></a><span data-ttu-id="fc4f7-103">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="fc4f7-103">Update contactfolder</span></span>

> <span data-ttu-id="fc4f7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc4f7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc4f7-106">Atualizar as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-106">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc4f7-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc4f7-107">Permissions</span></span>
<span data-ttu-id="fc4f7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc4f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc4f7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc4f7-110">Permission type</span></span>      | <span data-ttu-id="fc4f7-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc4f7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc4f7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc4f7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fc4f7-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc4f7-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fc4f7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc4f7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc4f7-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc4f7-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fc4f7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc4f7-116">Application</span></span> | <span data-ttu-id="fc4f7-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fc4f7-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc4f7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc4f7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fc4f7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc4f7-119">Request headers</span></span>
| <span data-ttu-id="fc4f7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fc4f7-120">Header</span></span>       | <span data-ttu-id="fc4f7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fc4f7-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc4f7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc4f7-122">Authorization</span></span>  | <span data-ttu-id="fc4f7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fc4f7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc4f7-125">Content-Type</span></span>  | <span data-ttu-id="fc4f7-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc4f7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc4f7-128">Request body</span></span>
<span data-ttu-id="fc4f7-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fc4f7-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc4f7-132">Property</span></span>     | <span data-ttu-id="fc4f7-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc4f7-133">Type</span></span>   |<span data-ttu-id="fc4f7-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc4f7-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc4f7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fc4f7-135">displayName</span></span>|<span data-ttu-id="fc4f7-136">String</span><span class="sxs-lookup"><span data-stu-id="fc4f7-136">String</span></span>|<span data-ttu-id="fc4f7-137">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-137">The folder's display name.</span></span>|
|<span data-ttu-id="fc4f7-138">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="fc4f7-138">parentFolderId</span></span>|<span data-ttu-id="fc4f7-139">String</span><span class="sxs-lookup"><span data-stu-id="fc4f7-139">String</span></span>|<span data-ttu-id="fc4f7-140">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-140">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="fc4f7-141">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="fc4f7-141">wellKnownName</span></span>|<span data-ttu-id="fc4f7-142">string</span><span class="sxs-lookup"><span data-stu-id="fc4f7-142">string</span></span>|<span data-ttu-id="fc4f7-143">O nome da pasta se a pasta for uma pasta reconhecida.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-143">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="fc4f7-144">No momento `contacts` é a única pasta Contatos reconhecidas.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-144">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="fc4f7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc4f7-145">Response</span></span>

<span data-ttu-id="fc4f7-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-146">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc4f7-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc4f7-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc4f7-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc4f7-148">Request</span></span>
<span data-ttu-id="fc4f7-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="fc4f7-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc4f7-150">Response</span></span>
<span data-ttu-id="fc4f7-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc4f7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "wellKnownName": "wellKnownName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
