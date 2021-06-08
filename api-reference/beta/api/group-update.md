---
title: Atualizar grupo
description: Atualize as propriedades de um [objeto group.](../resources/group.md)
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 39e1787ba3a88a0988977cb3c34d9575f608980a
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786942"
---
# <a name="update-group"></a><span data-ttu-id="cae5d-103">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="cae5d-103">Update group</span></span>

<span data-ttu-id="cae5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cae5d-105">Atualize as propriedades de um [objeto group.](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="cae5d-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cae5d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="cae5d-106">Permissions</span></span>

<span data-ttu-id="cae5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cae5d-109">Permission type</span></span>      | <span data-ttu-id="cae5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cae5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae5d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cae5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cae5d-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cae5d-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="cae5d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cae5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cae5d-114">Not supported.</span></span>    |
|<span data-ttu-id="cae5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cae5d-115">Application</span></span> | <span data-ttu-id="cae5d-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cae5d-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cae5d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cae5d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cae5d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cae5d-118">Request headers</span></span>

| <span data-ttu-id="cae5d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="cae5d-119">Name</span></span>       | <span data-ttu-id="cae5d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="cae5d-120">Type</span></span> | <span data-ttu-id="cae5d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cae5d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cae5d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cae5d-122">Authorization</span></span>  | <span data-ttu-id="cae5d-123">string</span><span class="sxs-lookup"><span data-stu-id="cae5d-123">string</span></span>  | <span data-ttu-id="cae5d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cae5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cae5d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cae5d-126">Request body</span></span>

<span data-ttu-id="cae5d-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cae5d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cae5d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cae5d-130">Property</span></span>   | <span data-ttu-id="cae5d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cae5d-131">Type</span></span> |<span data-ttu-id="cae5d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cae5d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cae5d-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="cae5d-133">allowExternalSenders</span></span>|<span data-ttu-id="cae5d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="cae5d-134">Boolean</span></span>|<span data-ttu-id="cae5d-135">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="cae5d-135">Default is `false`.</span></span> <span data-ttu-id="cae5d-136">Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.</span><span class="sxs-lookup"><span data-stu-id="cae5d-136">Indicates whether people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="cae5d-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="cae5d-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="cae5d-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="cae5d-138">Boolean</span></span>|<span data-ttu-id="cae5d-139">O padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="cae5d-139">Default is `false`.</span></span> <span data-ttu-id="cae5d-140">Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="cae5d-140">Indicates whether new members added to the group will be auto-subscribed to receive email notifications.</span></span> <span data-ttu-id="cae5d-141">**autoSubscribeNewMembers** não pode ser `true` quando **subscriptionEnabled** é definido como `false` no grupo.</span><span class="sxs-lookup"><span data-stu-id="cae5d-141">**autoSubscribeNewMembers** can't be `true` when **subscriptionEnabled** is set to `false` on the group.</span></span>|
|<span data-ttu-id="cae5d-142">descrição</span><span class="sxs-lookup"><span data-stu-id="cae5d-142">description</span></span>|<span data-ttu-id="cae5d-143">String</span><span class="sxs-lookup"><span data-stu-id="cae5d-143">String</span></span>|<span data-ttu-id="cae5d-144">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="cae5d-144">An optional description for the group.</span></span>|
|<span data-ttu-id="cae5d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="cae5d-145">displayName</span></span>|<span data-ttu-id="cae5d-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cae5d-146">String</span></span>|<span data-ttu-id="cae5d-p106">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="cae5d-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="cae5d-149">groupTypes</span><span class="sxs-lookup"><span data-stu-id="cae5d-149">groupTypes</span></span>|<span data-ttu-id="cae5d-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cae5d-150">String collection</span></span>|<span data-ttu-id="cae5d-151">Especifica o tipo de grupo e sua associação.</span><span class="sxs-lookup"><span data-stu-id="cae5d-151">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="cae5d-152">Se a coleção **contiver Unified,** o grupo será um Microsoft 365 grupo; caso contrário, é um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="cae5d-152">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise, it's a security group.</span></span>  <br><br><span data-ttu-id="cae5d-153">Se a coleção incluir **DynamicMembership**, o grupo tem associação dinâmica; caso contrário, a associação é estática.</span><span class="sxs-lookup"><span data-stu-id="cae5d-153">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="cae5d-154">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="cae5d-154">mailEnabled</span></span>|<span data-ttu-id="cae5d-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="cae5d-155">Boolean</span></span>|<span data-ttu-id="cae5d-156">Especifica se o grupo está habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="cae5d-156">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="cae5d-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="cae5d-157">mailNickname</span></span>|<span data-ttu-id="cae5d-158">String</span><span class="sxs-lookup"><span data-stu-id="cae5d-158">String</span></span>|<span data-ttu-id="cae5d-p107">O alias de e-mail do grupo. Essa propriedade deve ser especificada quando um grupo é criado. </span><span class="sxs-lookup"><span data-stu-id="cae5d-p107">The mail alias for the group. This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="cae5d-161">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="cae5d-161">securityEnabled</span></span>|<span data-ttu-id="cae5d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="cae5d-162">Boolean</span></span>|<span data-ttu-id="cae5d-163">Especifica se o grupo é um grupo de segurança, incluindo Microsoft 365 grupos.</span><span class="sxs-lookup"><span data-stu-id="cae5d-163">Specifies whether the group is a security group, including Microsoft 365 groups.</span></span> |
|<span data-ttu-id="cae5d-164">visibility</span><span class="sxs-lookup"><span data-stu-id="cae5d-164">visibility</span></span>|<span data-ttu-id="cae5d-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cae5d-165">String</span></span>|<span data-ttu-id="cae5d-166">Especifica a visibilidade de um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cae5d-166">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="cae5d-167">Os valores possíveis são: **Private**, **Public** ou vazio (que é interpretado como **Public**).</span><span class="sxs-lookup"><span data-stu-id="cae5d-167">Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="cae5d-168">Como o **recurso de** grupo dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância de grupo `PATCH` existente. </span><span class="sxs-lookup"><span data-stu-id="cae5d-168">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="cae5d-169">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="cae5d-169">**Note:**</span></span>
>
> - <span data-ttu-id="cae5d-170">Você pode atualizar o **autoSubscribeNewMembers** e **autoSubscribeNewMembers** especificando-os em sua própria solicitação de PATCH, sem incluir as outras propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="cae5d-170">You can update **allowExternalSenders** and **autoSubscribeNewMembers** by specifying them in their own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="cae5d-p109">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](/graph/known-issues#group).</span><span class="sxs-lookup"><span data-stu-id="cae5d-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](/graph/known-issues#group) for examples.</span></span>
> - <span data-ttu-id="cae5d-174">As regras para atualizar os grupos de segurança habilitados para email no Microsoft Exchange Server podem ser complexas; Para saber mais, confira [Gerenciar grupos de segurança habilitados para email no Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="cae5d-174">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="cae5d-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="cae5d-175">Response</span></span>

<span data-ttu-id="cae5d-176">Se for bem-sucedido, este método retorna um código de resposta `204 No Content`, exceto um código de resposta `200 OK` ao atualizar as seguintes propriedades: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span><span class="sxs-lookup"><span data-stu-id="cae5d-176">If successful, this method returns a `204 No Content` response code—except a `200 OK` response code when updating the following properties: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.</span></span>

## <a name="examples"></a><span data-ttu-id="cae5d-177">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cae5d-177">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="cae5d-178">Exemplo 1: atualizar o nome de exibição e a descrição de um grupo</span><span class="sxs-lookup"><span data-stu-id="cae5d-178">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="cae5d-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cae5d-179">Request</span></span>

<span data-ttu-id="cae5d-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cae5d-180">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cae5d-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae5d-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}
Content-type: application/json
Content-length: 211

{
   "description":"description-value",
   "displayName":"displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="cae5d-182">C#</span><span class="sxs-lookup"><span data-stu-id="cae5d-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cae5d-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae5d-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cae5d-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae5d-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cae5d-185">Java</span><span class="sxs-lookup"><span data-stu-id="cae5d-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cae5d-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="cae5d-186">Response</span></span>

<span data-ttu-id="cae5d-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cae5d-187">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a><span data-ttu-id="cae5d-188">Exemplo 2: aplicar o rótulo de sensibilidade a um Microsoft 365 grupo</span><span class="sxs-lookup"><span data-stu-id="cae5d-188">Example 2: Apply sensitivity label to a Microsoft 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="cae5d-189">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cae5d-189">Request</span></span>

<span data-ttu-id="cae5d-190">Você pode obter a ID do rótulo que deseja aplicar a um grupo Microsoft 365 usando [o rótulo lista](informationprotectionpolicy-list-labels.md).</span><span class="sxs-lookup"><span data-stu-id="cae5d-190">You can obtain the ID of the label you want to apply to a Microsoft 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="cae5d-191">Em seguida, você pode atualizar [a propriedade assignedLabels](../resources/assignedlabel.md) do grupo com a ID do rótulo.</span><span class="sxs-lookup"><span data-stu-id="cae5d-191">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 


# <a name="http"></a>[<span data-ttu-id="cae5d-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae5d-192">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cae5d-193">C#</span><span class="sxs-lookup"><span data-stu-id="cae5d-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cae5d-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae5d-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cae5d-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae5d-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cae5d-196">Java</span><span class="sxs-lookup"><span data-stu-id="cae5d-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cae5d-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="cae5d-197">Response</span></span>

<span data-ttu-id="cae5d-198">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cae5d-198">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="cae5d-199">Confira também</span><span class="sxs-lookup"><span data-stu-id="cae5d-199">See also</span></span>

- [<span data-ttu-id="cae5d-200">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="cae5d-200">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="cae5d-201">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="cae5d-201">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="cae5d-202">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="cae5d-202">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
