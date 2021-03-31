---
title: Atualizar grupo
description: Atualize as propriedades de um [objeto group.](../resources/group.md)
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 13d605efafb3d74cbaa78d79fb7fc634168b016a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468860"
---
# <a name="update-group"></a><span data-ttu-id="118eb-103">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="118eb-103">Update group</span></span>

<span data-ttu-id="118eb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="118eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="118eb-105">Atualize as propriedades de um [objeto group.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="118eb-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="118eb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="118eb-106">Permissions</span></span>

<span data-ttu-id="118eb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="118eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="118eb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="118eb-109">Permission type</span></span>      | <span data-ttu-id="118eb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="118eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="118eb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="118eb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="118eb-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="118eb-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="118eb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="118eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="118eb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="118eb-114">Not supported.</span></span>    |
|<span data-ttu-id="118eb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="118eb-115">Application</span></span> | <span data-ttu-id="118eb-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="118eb-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="118eb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="118eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="118eb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="118eb-118">Request headers</span></span>

| <span data-ttu-id="118eb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="118eb-119">Name</span></span>       | <span data-ttu-id="118eb-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="118eb-120">Type</span></span> | <span data-ttu-id="118eb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="118eb-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="118eb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="118eb-122">Authorization</span></span>  | <span data-ttu-id="118eb-123">string</span><span class="sxs-lookup"><span data-stu-id="118eb-123">string</span></span>  | <span data-ttu-id="118eb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="118eb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="118eb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="118eb-126">Request body</span></span>

<span data-ttu-id="118eb-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="118eb-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="118eb-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="118eb-130">Property</span></span>   | <span data-ttu-id="118eb-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="118eb-131">Type</span></span> |<span data-ttu-id="118eb-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="118eb-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="118eb-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="118eb-133">allowExternalSenders</span></span>|<span data-ttu-id="118eb-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="118eb-134">Boolean</span></span>|<span data-ttu-id="118eb-135">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="118eb-135">Default is `false`.</span></span> <span data-ttu-id="118eb-136">Indica se as pessoas externas à organização podem enviar mensagens para o grupo.</span><span class="sxs-lookup"><span data-stu-id="118eb-136">Indicates whether people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="118eb-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="118eb-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="118eb-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="118eb-138">Boolean</span></span>|<span data-ttu-id="118eb-139">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="118eb-139">Default is `false`.</span></span> <span data-ttu-id="118eb-140">Indica se novos membros adicionados ao grupo serão inscritos automaticamente para receber notificações por email.</span><span class="sxs-lookup"><span data-stu-id="118eb-140">Indicates whether new members added to the group will be auto-subscribed to receive email notifications.</span></span> <span data-ttu-id="118eb-141">**autoSubscribeNewMembers** não pode ser quando `true` **subscriptionEnabled** é `false` definido como no grupo.</span><span class="sxs-lookup"><span data-stu-id="118eb-141">**autoSubscribeNewMembers** can't be `true` when **subscriptionEnabled** is set to `false` on the group.</span></span>|
|<span data-ttu-id="118eb-142">descrição</span><span class="sxs-lookup"><span data-stu-id="118eb-142">description</span></span>|<span data-ttu-id="118eb-143">String</span><span class="sxs-lookup"><span data-stu-id="118eb-143">String</span></span>|<span data-ttu-id="118eb-144">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="118eb-144">An optional description for the group.</span></span>|
|<span data-ttu-id="118eb-145">descrição</span><span class="sxs-lookup"><span data-stu-id="118eb-145">description</span></span>|<span data-ttu-id="118eb-146">String</span><span class="sxs-lookup"><span data-stu-id="118eb-146">String</span></span>|<span data-ttu-id="118eb-147">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="118eb-147">An optional description for the group.</span></span> |
|<span data-ttu-id="118eb-148">displayName</span><span class="sxs-lookup"><span data-stu-id="118eb-148">displayName</span></span>|<span data-ttu-id="118eb-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="118eb-149">String</span></span>|<span data-ttu-id="118eb-p106">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="118eb-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="118eb-152">groupTypes</span><span class="sxs-lookup"><span data-stu-id="118eb-152">groupTypes</span></span>|<span data-ttu-id="118eb-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="118eb-153">String collection</span></span>|<span data-ttu-id="118eb-154">Especifica o tipo de grupo e sua associação.</span><span class="sxs-lookup"><span data-stu-id="118eb-154">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="118eb-155">Se a coleção contiver um grupo **unificado** então o grupo será um grupo do Microsoft 365; caso contrário, será um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="118eb-155">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="118eb-156">Se a coleção incluir **DynamicMembership**, o grupo tem associação dinâmica; caso contrário, a associação é estática.</span><span class="sxs-lookup"><span data-stu-id="118eb-156">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="118eb-157">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="118eb-157">mailEnabled</span></span>|<span data-ttu-id="118eb-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="118eb-158">Boolean</span></span>|<span data-ttu-id="118eb-159">Especifica se o grupo está habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="118eb-159">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="118eb-160">mailNickname</span><span class="sxs-lookup"><span data-stu-id="118eb-160">mailNickname</span></span>|<span data-ttu-id="118eb-161">String</span><span class="sxs-lookup"><span data-stu-id="118eb-161">String</span></span>|<span data-ttu-id="118eb-162">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="118eb-162">The mail alias for the group.</span></span> <span data-ttu-id="118eb-163">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="118eb-163">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="118eb-164">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="118eb-164">securityEnabled</span></span>|<span data-ttu-id="118eb-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="118eb-165">Boolean</span></span>|<span data-ttu-id="118eb-166">Especifica se o grupo é um grupo de segurança, incluindo grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="118eb-166">Specifies whether the group is a security group, including Microsoft 365 groups.</span></span> |
|<span data-ttu-id="118eb-167">visibility</span><span class="sxs-lookup"><span data-stu-id="118eb-167">visibility</span></span>|<span data-ttu-id="118eb-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="118eb-168">String</span></span>|<span data-ttu-id="118eb-169">Especifica a visibilidade de um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="118eb-169">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="118eb-170">Os valores possíveis são: **Private**, **Public** ou vazio (que é interpretado como **Public**).</span><span class="sxs-lookup"><span data-stu-id="118eb-170">Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="118eb-171">Como o **recurso de** grupo dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância de grupo `PATCH` existente. </span><span class="sxs-lookup"><span data-stu-id="118eb-171">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="118eb-172">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="118eb-172">**Note:**</span></span>
>
> - <span data-ttu-id="118eb-173">Você pode atualizar **allowExternalSenders** e **autoSubscribeNewMembers** especificando-os em sua própria solicitação PATCH, sem incluir as outras propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="118eb-173">You can update **allowExternalSenders** and **autoSubscribeNewMembers** by specifying them in their own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="118eb-p109">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](/graph/known-issues#group).</span><span class="sxs-lookup"><span data-stu-id="118eb-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](/graph/known-issues#group) for examples.</span></span>
> - <span data-ttu-id="118eb-177">As regras para atualizar os grupos de segurança habilitados para email no Microsoft Exchange Server podem ser complexas; Para saber mais, confira [Gerenciar grupos de segurança habilitados para email no Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="118eb-177">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="118eb-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="118eb-178">Response</span></span>

<span data-ttu-id="118eb-179">Se tiver êxito, este método retornará um código de resposta, exceto um código de resposta ao atualizar as seguintes `204 No Content` `200 OK` propriedades: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span><span class="sxs-lookup"><span data-stu-id="118eb-179">If successful, this method returns a `204 No Content` response code—except a `200 OK` response code when updating the following properties: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span></span>

## <a name="examples"></a><span data-ttu-id="118eb-180">Exemplos</span><span class="sxs-lookup"><span data-stu-id="118eb-180">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="118eb-181">Exemplo 1: atualizar o nome de exibição e a descrição de um grupo</span><span class="sxs-lookup"><span data-stu-id="118eb-181">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="118eb-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="118eb-182">Request</span></span>

<span data-ttu-id="118eb-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="118eb-183">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="118eb-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="118eb-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "description": "description-value",
  "displayName": "displayName-value",
}
```
# <a name="c"></a>[<span data-ttu-id="118eb-185">C#</span><span class="sxs-lookup"><span data-stu-id="118eb-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="118eb-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="118eb-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="118eb-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="118eb-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="118eb-188">Java</span><span class="sxs-lookup"><span data-stu-id="118eb-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="118eb-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="118eb-189">Response</span></span>

<span data-ttu-id="118eb-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="118eb-190">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a><span data-ttu-id="118eb-191">Exemplo 2: aplicar o rótulo de sensibilidade a um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="118eb-191">Example 2: Apply sensitivity label to a Microsoft 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="118eb-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="118eb-192">Request</span></span>

<span data-ttu-id="118eb-193">Você pode obter a ID do rótulo que deseja aplicar a um grupo do Microsoft 365 usando [List label](informationprotectionpolicy-list-labels.md).</span><span class="sxs-lookup"><span data-stu-id="118eb-193">You can obtain the ID of the label you want to apply to a Microsoft 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="118eb-194">Em seguida, você pode atualizar [a propriedade assignedLabels](../resources/assignedlabel.md) do grupo com a ID do rótulo.</span><span class="sxs-lookup"><span data-stu-id="118eb-194">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 


# <a name="http"></a>[<span data-ttu-id="118eb-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="118eb-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
  "assignedLabels": 
  [
    {
        "labelId" : "45cd0c48-c540-4358-ad79-a3658cdc5b88"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="118eb-196">C#</span><span class="sxs-lookup"><span data-stu-id="118eb-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="118eb-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="118eb-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="118eb-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="118eb-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="118eb-199">Java</span><span class="sxs-lookup"><span data-stu-id="118eb-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="118eb-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="118eb-200">Response</span></span>

<span data-ttu-id="118eb-201">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="118eb-201">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="118eb-202">Confira também</span><span class="sxs-lookup"><span data-stu-id="118eb-202">See also</span></span>

- [<span data-ttu-id="118eb-203">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="118eb-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="118eb-204">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="118eb-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="118eb-205">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="118eb-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
