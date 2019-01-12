---
title: Atualizar contactfolder
description: Atualizar as propriedades do objeto contactfolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9b2244f17bf877c1f52ae5de812f65ba1eae3b98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956147"
---
# <a name="update-contactfolder"></a><span data-ttu-id="fd9e1-103">Atualizar contactfolder</span><span class="sxs-lookup"><span data-stu-id="fd9e1-103">Update contactfolder</span></span>

> <span data-ttu-id="fd9e1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd9e1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd9e1-106">Atualizar as propriedades do objeto contactfolder.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-106">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fd9e1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd9e1-107">Permissions</span></span>
<span data-ttu-id="fd9e1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd9e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd9e1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd9e1-110">Permission type</span></span>      | <span data-ttu-id="fd9e1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd9e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd9e1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd9e1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd9e1-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd9e1-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fd9e1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd9e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd9e1-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd9e1-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="fd9e1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd9e1-116">Application</span></span> | <span data-ttu-id="fd9e1-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd9e1-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd9e1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd9e1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fd9e1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd9e1-119">Request headers</span></span>
| <span data-ttu-id="fd9e1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fd9e1-120">Header</span></span>       | <span data-ttu-id="fd9e1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fd9e1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd9e1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd9e1-122">Authorization</span></span>  | <span data-ttu-id="fd9e1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fd9e1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fd9e1-125">Content-Type</span></span>  | <span data-ttu-id="fd9e1-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd9e1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd9e1-128">Request body</span></span>
<span data-ttu-id="fd9e1-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fd9e1-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd9e1-132">Property</span></span>     | <span data-ttu-id="fd9e1-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd9e1-133">Type</span></span>   |<span data-ttu-id="fd9e1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd9e1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd9e1-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fd9e1-135">displayName</span></span>|<span data-ttu-id="fd9e1-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd9e1-136">String</span></span>|<span data-ttu-id="fd9e1-137">O nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-137">The folder's display name.</span></span>|
|<span data-ttu-id="fd9e1-138">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="fd9e1-138">parentFolderId</span></span>|<span data-ttu-id="fd9e1-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd9e1-139">String</span></span>|<span data-ttu-id="fd9e1-140">A ID da pasta pai da pasta.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-140">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="fd9e1-141">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="fd9e1-141">wellKnownName</span></span>|<span data-ttu-id="fd9e1-142">string</span><span class="sxs-lookup"><span data-stu-id="fd9e1-142">string</span></span>|<span data-ttu-id="fd9e1-143">O nome da pasta se a pasta for uma pasta reconhecida.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-143">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="fd9e1-144">No momento `contacts` é a única pasta Contatos reconhecidas.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-144">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="fd9e1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd9e1-145">Response</span></span>

<span data-ttu-id="fd9e1-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [contactFolder](../resources/contactfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-146">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd9e1-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd9e1-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd9e1-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd9e1-148">Request</span></span>
<span data-ttu-id="fd9e1-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-149">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fd9e1-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd9e1-150">Response</span></span>
<span data-ttu-id="fd9e1-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd9e1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
