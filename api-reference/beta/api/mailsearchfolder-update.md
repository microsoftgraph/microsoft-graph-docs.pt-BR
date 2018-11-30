---
title: Atualizar mailSearchFolder
description: Atualize as propriedades graváveis do objeto mailSearchFolder.
ms.openlocfilehash: abe32817c45ee1e05fbb251bd46a31941eb4218b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041177"
---
# <a name="update-mailsearchfolder"></a><span data-ttu-id="745b5-103">Atualizar mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="745b5-103">Update mailSearchFolder</span></span>

> <span data-ttu-id="745b5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="745b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="745b5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="745b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="745b5-106">Atualize as propriedades graváveis do objeto [mailSearchFolder](../resources/mailsearchfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="745b5-106">Update the writable properties of [mailSearchFolder](../resources/mailsearchfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="745b5-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="745b5-107">Permissions</span></span>
<span data-ttu-id="745b5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="745b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="745b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="745b5-110">Permission type</span></span>      | <span data-ttu-id="745b5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="745b5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="745b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="745b5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="745b5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="745b5-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="745b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="745b5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="745b5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="745b5-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="745b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="745b5-116">Application</span></span> | <span data-ttu-id="745b5-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="745b5-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="745b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="745b5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="745b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="745b5-119">Request headers</span></span>
| <span data-ttu-id="745b5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="745b5-120">Header</span></span>       | <span data-ttu-id="745b5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="745b5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="745b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="745b5-122">Authorization</span></span>  | <span data-ttu-id="745b5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="745b5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="745b5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="745b5-125">Content-Type</span></span>  | <span data-ttu-id="745b5-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="745b5-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="745b5-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="745b5-128">Request body</span></span>
<span data-ttu-id="745b5-p105">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="745b5-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="745b5-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="745b5-132">Property</span></span>     | <span data-ttu-id="745b5-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="745b5-133">Type</span></span>   |<span data-ttu-id="745b5-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="745b5-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="745b5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="745b5-135">displayName</span></span> | <span data-ttu-id="745b5-136">String</span><span class="sxs-lookup"><span data-stu-id="745b5-136">String</span></span> | <span data-ttu-id="745b5-137">O nome de exibição do [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="745b5-137">The display name of the [mailFolder](../resources/mailfolder.md).</span></span>|
| <span data-ttu-id="745b5-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="745b5-138">includeNestedFolders</span></span> | <span data-ttu-id="745b5-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="745b5-139">Boolean</span></span> | <span data-ttu-id="745b5-140">Como a hierarquia de pastas de caixa de correio deve ser percorrida.</span><span class="sxs-lookup"><span data-stu-id="745b5-140">How the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="745b5-141">`true`significa que uma profundidade de pesquisa deve ser feito ao `false` significa rasos de pesquisa devem ser feito em vez disso.</span><span class="sxs-lookup"><span data-stu-id="745b5-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="745b5-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="745b5-142">sourceFolderIDs</span></span> | <span data-ttu-id="745b5-143">String collection</span><span class="sxs-lookup"><span data-stu-id="745b5-143">String collection</span></span> | <span data-ttu-id="745b5-144">As pastas de caixa de correio que devem ser extraídas.</span><span class="sxs-lookup"><span data-stu-id="745b5-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="745b5-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="745b5-145">filterQuery</span></span> | <span data-ttu-id="745b5-146">String</span><span class="sxs-lookup"><span data-stu-id="745b5-146">String</span></span> | <span data-ttu-id="745b5-147">A consulta OData para filtrar as mensagens.</span><span class="sxs-lookup"><span data-stu-id="745b5-147">The OData query to filter the messages.</span></span> |

## <a name="response"></a><span data-ttu-id="745b5-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="745b5-148">Response</span></span>
<span data-ttu-id="745b5-149">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [mailFolder](../resources/mailfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="745b5-149">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="745b5-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="745b5-150">Example</span></span>
#### <a name="request"></a><span data-ttu-id="745b5-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="745b5-151">Request</span></span>
<span data-ttu-id="745b5-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="745b5-152">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailsearchfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "filterQuery": "contains(subject, 'Analytics')))"
}
```

#### <a name="response"></a><span data-ttu-id="745b5-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="745b5-153">Response</span></span>
<span data-ttu-id="745b5-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="745b5-154">The following is an example of the response.</span></span>
><span data-ttu-id="745b5-155">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="745b5-155">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="745b5-156">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="745b5-156">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzMx",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzMy",
  "childFolderCount": 0,
  "unreadItemCount": 0,
  "totalItemCount": 0,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": [
      "AAMkAGVmMDEzMi"
  ],
  "filterQuery": "contains(subject, 'Analytics')"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailSearchFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
