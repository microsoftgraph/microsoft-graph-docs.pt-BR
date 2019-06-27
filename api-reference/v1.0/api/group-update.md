---
title: Atualizar grupo
description: Atualizar as propriedades de um objeto group.
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 9f6ddca037452003b0192cf7b3cdcd894d2d03f0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263551"
---
# <a name="update-group"></a><span data-ttu-id="950de-103">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="950de-103">Update group</span></span>

<span data-ttu-id="950de-104">Atualizar as propriedades de um objeto group.</span><span class="sxs-lookup"><span data-stu-id="950de-104">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="950de-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="950de-105">Permissions</span></span>

<span data-ttu-id="950de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="950de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="950de-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="950de-108">Permission type</span></span>      | <span data-ttu-id="950de-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="950de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="950de-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="950de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="950de-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="950de-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="950de-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="950de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="950de-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="950de-113">Not supported.</span></span>    |
|<span data-ttu-id="950de-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="950de-114">Application</span></span> | <span data-ttu-id="950de-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="950de-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="950de-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="950de-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="950de-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="950de-117">Request headers</span></span>

| <span data-ttu-id="950de-118">Nome</span><span class="sxs-lookup"><span data-stu-id="950de-118">Name</span></span>       | <span data-ttu-id="950de-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="950de-119">Type</span></span> | <span data-ttu-id="950de-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="950de-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="950de-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="950de-121">Authorization</span></span>  | <span data-ttu-id="950de-122">string</span><span class="sxs-lookup"><span data-stu-id="950de-122">string</span></span>  | <span data-ttu-id="950de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="950de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="950de-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="950de-125">Request body</span></span>

<span data-ttu-id="950de-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="950de-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="950de-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="950de-129">Property</span></span>   | <span data-ttu-id="950de-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="950de-130">Type</span></span> |<span data-ttu-id="950de-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="950de-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="950de-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="950de-132">allowExternalSenders</span></span>|<span data-ttu-id="950de-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="950de-133">Boolean</span></span>|<span data-ttu-id="950de-p104">O padrão é **false**. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.</span><span class="sxs-lookup"><span data-stu-id="950de-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="950de-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="950de-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="950de-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="950de-137">Boolean</span></span>|<span data-ttu-id="950de-p105">O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="950de-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="950de-140">description</span><span class="sxs-lookup"><span data-stu-id="950de-140">description</span></span>|<span data-ttu-id="950de-141">String</span><span class="sxs-lookup"><span data-stu-id="950de-141">String</span></span>|<span data-ttu-id="950de-142">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="950de-142">An optional description for the group.</span></span> |
|<span data-ttu-id="950de-143">displayName</span><span class="sxs-lookup"><span data-stu-id="950de-143">displayName</span></span>|<span data-ttu-id="950de-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="950de-144">String</span></span>|<span data-ttu-id="950de-p106">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="950de-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span> |
|<span data-ttu-id="950de-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="950de-147">groupTypes</span></span>|<span data-ttu-id="950de-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="950de-148">String collection</span></span>|<span data-ttu-id="950de-149">Especifica o tipo de grupo e sua associação.</span><span class="sxs-lookup"><span data-stu-id="950de-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="950de-150">Se a coleção contiver **Unificado** o grupo será um grupo do Office 365; caso contrário, será um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="950de-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="950de-151">Se a coleção incluir **DynamicMembership**, o grupo tem associação dinâmica; caso contrário, a associação é estática.</span><span class="sxs-lookup"><span data-stu-id="950de-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="950de-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="950de-152">mailEnabled</span></span>|<span data-ttu-id="950de-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="950de-153">Boolean</span></span>|<span data-ttu-id="950de-154">Especifica se o grupo está habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="950de-154">Specifies whether the group is a security group.</span></span>|
|<span data-ttu-id="950de-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="950de-155">mailNickname</span></span>|<span data-ttu-id="950de-156">String</span><span class="sxs-lookup"><span data-stu-id="950de-156">String</span></span>|<span data-ttu-id="950de-157">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="950de-157">The mail alias for the group.</span></span> <span data-ttu-id="950de-158">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="950de-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="950de-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="950de-159">securityEnabled</span></span>|<span data-ttu-id="950de-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="950de-160">Boolean</span></span>|<span data-ttu-id="950de-161">Especifica se o grupo é um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="950de-161">Specifies whether the group is a security group.</span></span> |
|<span data-ttu-id="950de-162">visibility</span><span class="sxs-lookup"><span data-stu-id="950de-162">visibility</span></span>|<span data-ttu-id="950de-163">String</span><span class="sxs-lookup"><span data-stu-id="950de-163">String</span></span>|<span data-ttu-id="950de-164">Especifica a visibilidade de um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="950de-164">Specifies the visibility of an Office 365 group.</span></span> <span data-ttu-id="950de-165">Os valores possíveis são: **Privado**, **Público** ou vazio (que é interpretado como **Público**).</span><span class="sxs-lookup"><span data-stu-id="950de-165">The possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

> <span data-ttu-id="950de-166">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="950de-166">**Note:**</span></span>
>
> - <span data-ttu-id="950de-167">Você pode atualizar o **autoSubscribeNewMembers** especificando-o em sua própria solicitação de PATCH, sem incluir as outras propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="950de-167">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request,without including the other properties in the table above.</span></span>
> - <span data-ttu-id="950de-p109">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="950de-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="950de-171">As regras para atualizar os grupos de segurança habilitados para email no Microsoft Exchange Server podem ser complexas; Para saber mais, confira [Gerenciar grupos de segurança habilitados para email no Exchange Server](https://docs.microsoft.com/pt-BR/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="950de-171">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](https://docs.microsoft.com/en-us/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>


## <a name="response"></a><span data-ttu-id="950de-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="950de-172">Response</span></span>

<span data-ttu-id="950de-173">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="950de-173">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="950de-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="950de-174">Example</span></span>

<span data-ttu-id="950de-175">O exemplo a seguir mostra como criar um grupo.</span><span class="sxs-lookup"><span data-stu-id="950de-175">The following example shows how to create a calculated field.</span></span>

### <a name="request"></a><span data-ttu-id="950de-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="950de-176">Request</span></span>

<span data-ttu-id="950de-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="950de-177">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_group"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```

### <a name="response"></a><span data-ttu-id="950de-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="950de-178">Response</span></span>

<span data-ttu-id="950de-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="950de-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="950de-180">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="950de-180">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="950de-181">C#</span><span class="sxs-lookup"><span data-stu-id="950de-181">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="950de-182">Javascript</span><span class="sxs-lookup"><span data-stu-id="950de-182">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="950de-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="950de-183">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
