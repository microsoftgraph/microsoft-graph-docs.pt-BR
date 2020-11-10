---
title: Atualizar grupo
description: Atualiza as propriedades de um objeto [Group](../resources/group.md) .
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ca2f6815f1206807d680100c04951bec6115ea91
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953743"
---
# <a name="update-group"></a><span data-ttu-id="becae-103">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="becae-103">Update group</span></span>

<span data-ttu-id="becae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="becae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="becae-105">Atualiza as propriedades de um objeto [Group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="becae-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="becae-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="becae-106">Permissions</span></span>

<span data-ttu-id="becae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="becae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="becae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="becae-109">Permission type</span></span>      | <span data-ttu-id="becae-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="becae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="becae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="becae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="becae-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="becae-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="becae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="becae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="becae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="becae-114">Not supported.</span></span>    |
|<span data-ttu-id="becae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="becae-115">Application</span></span> | <span data-ttu-id="becae-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="becae-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="becae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="becae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="becae-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="becae-118">Request headers</span></span>

| <span data-ttu-id="becae-119">Nome</span><span class="sxs-lookup"><span data-stu-id="becae-119">Name</span></span>       | <span data-ttu-id="becae-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="becae-120">Type</span></span> | <span data-ttu-id="becae-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="becae-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="becae-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="becae-122">Authorization</span></span>  | <span data-ttu-id="becae-123">string</span><span class="sxs-lookup"><span data-stu-id="becae-123">string</span></span>  | <span data-ttu-id="becae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="becae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="becae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="becae-126">Request body</span></span>

<span data-ttu-id="becae-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="becae-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="becae-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="becae-130">Property</span></span>   | <span data-ttu-id="becae-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="becae-131">Type</span></span> |<span data-ttu-id="becae-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="becae-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="becae-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="becae-133">allowExternalSenders</span></span>|<span data-ttu-id="becae-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="becae-134">Boolean</span></span>|<span data-ttu-id="becae-p104">O padrão é **false**. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.</span><span class="sxs-lookup"><span data-stu-id="becae-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="becae-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="becae-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="becae-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="becae-138">Boolean</span></span>|<span data-ttu-id="becae-p105">O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="becae-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="becae-141">description</span><span class="sxs-lookup"><span data-stu-id="becae-141">description</span></span>|<span data-ttu-id="becae-142">String</span><span class="sxs-lookup"><span data-stu-id="becae-142">String</span></span>|<span data-ttu-id="becae-143">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="becae-143">An optional description for the group.</span></span> |
|<span data-ttu-id="becae-144">displayName</span><span class="sxs-lookup"><span data-stu-id="becae-144">displayName</span></span>|<span data-ttu-id="becae-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="becae-145">String</span></span>|<span data-ttu-id="becae-p106">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="becae-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="becae-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="becae-148">groupTypes</span></span>|<span data-ttu-id="becae-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="becae-149">String collection</span></span>|<span data-ttu-id="becae-150">Especifica o tipo de grupo e sua associação.</span><span class="sxs-lookup"><span data-stu-id="becae-150">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="becae-151">Se a coleção contiver um grupo **unificado** então o grupo será um grupo do Microsoft 365; caso contrário, será um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="becae-151">If the collection contains **Unified** then the group is a Microsoft 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="becae-152">Se a coleção incluir **DynamicMembership** , o grupo tem associação dinâmica; caso contrário, a associação é estática.</span><span class="sxs-lookup"><span data-stu-id="becae-152">If the collection includes **DynamicMembership** , the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="becae-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="becae-153">mailEnabled</span></span>|<span data-ttu-id="becae-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="becae-154">Boolean</span></span>|<span data-ttu-id="becae-155">Especifica se o grupo está habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="becae-155">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="becae-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="becae-156">mailNickname</span></span>|<span data-ttu-id="becae-157">String</span><span class="sxs-lookup"><span data-stu-id="becae-157">String</span></span>|<span data-ttu-id="becae-158">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="becae-158">The mail alias for the group.</span></span> <span data-ttu-id="becae-159">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="becae-159">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="becae-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="becae-160">securityEnabled</span></span>|<span data-ttu-id="becae-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="becae-161">Boolean</span></span>|<span data-ttu-id="becae-162">Especifica se o grupo é um grupo de segurança, incluindo os grupos do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="becae-162">Specifies whether the group is a security group, including Microsoft 365 groups.</span></span> |
|<span data-ttu-id="becae-163">visibility</span><span class="sxs-lookup"><span data-stu-id="becae-163">visibility</span></span>|<span data-ttu-id="becae-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="becae-164">String</span></span>|<span data-ttu-id="becae-165">Especifica a visibilidade de um grupo do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="becae-165">Specifies the visibility of a Microsoft 365 group.</span></span> <span data-ttu-id="becae-166">Os valores possíveis são: **Private** , **Public** ou vazio (que é interpretado como **Public** ).</span><span class="sxs-lookup"><span data-stu-id="becae-166">Possible values are: **Private** , **Public** , or empty (which is interpreted as **Public** ).</span></span>|

<span data-ttu-id="becae-167">Como o recurso de **grupo** suporta [extensões](/graph/extensibility-overview), você pode usar a `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **grupo** existente.</span><span class="sxs-lookup"><span data-stu-id="becae-167">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="becae-168">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="becae-168">**Note:**</span></span>
>
> - <span data-ttu-id="becae-169">Você pode atualizar o **autoSubscribeNewMembers** especificando-o em sua própria solicitação PATCH, sem incluir as demais propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="becae-169">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="becae-p109">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers** , dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](/graph/known-issues#group).</span><span class="sxs-lookup"><span data-stu-id="becae-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers** , support only delegated permissions. See [known issues](/graph/known-issues#group) for examples.</span></span>
> - <span data-ttu-id="becae-173">As regras para atualizar os grupos de segurança habilitados para email no Microsoft Exchange Server podem ser complexas; Para saber mais, confira [Gerenciar grupos de segurança habilitados para email no Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="becae-173">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="becae-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="becae-174">Response</span></span>

<span data-ttu-id="becae-175">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="becae-175">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="becae-176">Exemplos</span><span class="sxs-lookup"><span data-stu-id="becae-176">Examples</span></span>

### <a name="example-1-update-display-name-and-description-of-a-group"></a><span data-ttu-id="becae-177">Exemplo 1: atualizar o nome de exibição e a descrição de um grupo</span><span class="sxs-lookup"><span data-stu-id="becae-177">Example 1: Update display name and description of a group</span></span>
#### <a name="request"></a><span data-ttu-id="becae-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="becae-178">Request</span></span>

<span data-ttu-id="becae-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="becae-179">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="becae-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="becae-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_group"
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
# <a name="c"></a>[<span data-ttu-id="becae-181">C#</span><span class="sxs-lookup"><span data-stu-id="becae-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="becae-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="becae-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="becae-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="becae-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="becae-184">Java</span><span class="sxs-lookup"><span data-stu-id="becae-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="becae-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="becae-185">Response</span></span>

<span data-ttu-id="becae-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="becae-186">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-2-apply-sensitivity-label-to-a-microsoft-365-group"></a><span data-ttu-id="becae-187">Exemplo 2: Aplicar rótulo de confidencialidade a um grupo do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="becae-187">Example 2: Apply sensitivity label to a Microsoft 365 group</span></span>
#### <a name="request"></a><span data-ttu-id="becae-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="becae-188">Request</span></span>

<span data-ttu-id="becae-189">Você pode obter a ID do rótulo que você deseja aplicar a um grupo do Microsoft 365 usando [rótulo de lista](informationprotectionpolicy-list-labels.md).</span><span class="sxs-lookup"><span data-stu-id="becae-189">You can obtain the ID of the label you want to apply to a Microsoft 365 group by using [List label](informationprotectionpolicy-list-labels.md).</span></span> <span data-ttu-id="becae-190">Em seguida, você pode atualizar a propriedade [assignedLabels](../resources/assignedlabel.md) do grupo com a ID de rótulo.</span><span class="sxs-lookup"><span data-stu-id="becae-190">Then you can update the [assignedLabels](../resources/assignedlabel.md) property of the group with the label ID.</span></span> 

<!-- {
  "blockType": "request",
  "name": "update_group"
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

#### <a name="response"></a><span data-ttu-id="becae-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="becae-191">Response</span></span>

<span data-ttu-id="becae-192">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="becae-192">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="becae-193">Confira também</span><span class="sxs-lookup"><span data-stu-id="becae-193">See also</span></span>

- [<span data-ttu-id="becae-194">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="becae-194">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="becae-195">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="becae-195">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="becae-196">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="becae-196">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
