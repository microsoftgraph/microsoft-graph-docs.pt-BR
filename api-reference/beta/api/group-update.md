---
title: Atualizar grupo
description: Atualiza as propriedades de um objeto [Group](../resources/group.md) .
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a2e5e9fa10ec8d37099f09cc294b36a429bb0642
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446678"
---
# <a name="update-group"></a><span data-ttu-id="ace89-103">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="ace89-103">Update group</span></span>

<span data-ttu-id="ace89-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ace89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ace89-105">Atualiza as propriedades de um objeto [Group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="ace89-105">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ace89-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ace89-106">Permissions</span></span>

<span data-ttu-id="ace89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace89-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ace89-109">Permission type</span></span>      | <span data-ttu-id="ace89-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ace89-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ace89-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ace89-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ace89-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ace89-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="ace89-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ace89-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ace89-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ace89-114">Not supported.</span></span>    |
|<span data-ttu-id="ace89-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ace89-115">Application</span></span> | <span data-ttu-id="ace89-116">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace89-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ace89-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ace89-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ace89-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ace89-118">Request headers</span></span>

| <span data-ttu-id="ace89-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ace89-119">Name</span></span>       | <span data-ttu-id="ace89-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ace89-120">Type</span></span> | <span data-ttu-id="ace89-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ace89-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ace89-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ace89-122">Authorization</span></span>  | <span data-ttu-id="ace89-123">string</span><span class="sxs-lookup"><span data-stu-id="ace89-123">string</span></span>  | <span data-ttu-id="ace89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ace89-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ace89-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ace89-126">Request body</span></span>

<span data-ttu-id="ace89-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ace89-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ace89-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ace89-130">Property</span></span>   | <span data-ttu-id="ace89-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ace89-131">Type</span></span> |<span data-ttu-id="ace89-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ace89-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ace89-133">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="ace89-133">allowExternalSenders</span></span>|<span data-ttu-id="ace89-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="ace89-134">Boolean</span></span>|<span data-ttu-id="ace89-p104">O padrão é **false**. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.</span><span class="sxs-lookup"><span data-stu-id="ace89-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="ace89-137">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="ace89-137">autoSubscribeNewMembers</span></span>|<span data-ttu-id="ace89-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="ace89-138">Boolean</span></span>|<span data-ttu-id="ace89-p105">O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="ace89-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="ace89-141">description</span><span class="sxs-lookup"><span data-stu-id="ace89-141">description</span></span>|<span data-ttu-id="ace89-142">String</span><span class="sxs-lookup"><span data-stu-id="ace89-142">String</span></span>|<span data-ttu-id="ace89-143">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="ace89-143">An optional description for the group.</span></span> |
|<span data-ttu-id="ace89-144">displayName</span><span class="sxs-lookup"><span data-stu-id="ace89-144">displayName</span></span>|<span data-ttu-id="ace89-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ace89-145">String</span></span>|<span data-ttu-id="ace89-p106">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="ace89-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="ace89-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="ace89-148">groupTypes</span></span>|<span data-ttu-id="ace89-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ace89-149">String collection</span></span>|<span data-ttu-id="ace89-150">Especifica o tipo de grupo e sua associação.</span><span class="sxs-lookup"><span data-stu-id="ace89-150">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="ace89-151">Se a coleção contiver **Unificado** o grupo será um grupo do Office 365; caso contrário, será um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="ace89-151">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="ace89-152">Se a coleção incluir **DynamicMembership**, o grupo tem associação dinâmica; caso contrário, a associação é estática.</span><span class="sxs-lookup"><span data-stu-id="ace89-152">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="ace89-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="ace89-153">mailEnabled</span></span>|<span data-ttu-id="ace89-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="ace89-154">Boolean</span></span>|<span data-ttu-id="ace89-155">Especifica se o grupo está habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="ace89-155">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="ace89-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ace89-156">mailNickname</span></span>|<span data-ttu-id="ace89-157">String</span><span class="sxs-lookup"><span data-stu-id="ace89-157">String</span></span>|<span data-ttu-id="ace89-158">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="ace89-158">The mail alias for the group.</span></span> <span data-ttu-id="ace89-159">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="ace89-159">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="ace89-160">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="ace89-160">securityEnabled</span></span>|<span data-ttu-id="ace89-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ace89-161">Boolean</span></span>|<span data-ttu-id="ace89-162">Especifica se o grupo é um grupo de segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="ace89-162">Specifies whether the group is a security group, including Office 365 groups.</span></span> |
|<span data-ttu-id="ace89-163">visibility</span><span class="sxs-lookup"><span data-stu-id="ace89-163">visibility</span></span>|<span data-ttu-id="ace89-164">String</span><span class="sxs-lookup"><span data-stu-id="ace89-164">String</span></span>|<span data-ttu-id="ace89-p108">Especifica a visibilidade de um grupo do Office 365. Os valores possíveis são: **Private**, **Public** ou vazio (que é interpretado como **Public**).</span><span class="sxs-lookup"><span data-stu-id="ace89-p108">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="ace89-167">Como o recurso de **grupo** suporta [extensões](/graph/extensibility-overview), você pode usar `PATCH` a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **grupo** existente.</span><span class="sxs-lookup"><span data-stu-id="ace89-167">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="ace89-168">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="ace89-168">**Note:**</span></span>
>
> - <span data-ttu-id="ace89-169">Você pode atualizar o **autoSubscribeNewMembers** especificando-o em sua própria solicitação PATCH, sem incluir as demais propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="ace89-169">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="ace89-p109">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="ace89-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="ace89-173">As regras para atualizar os grupos de segurança habilitados para email no Microsoft Exchange Server podem ser complexas; Para saber mais, confira [Gerenciar grupos de segurança habilitados para email no Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="ace89-173">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="ace89-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="ace89-174">Response</span></span>

<span data-ttu-id="ace89-175">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ace89-175">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ace89-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ace89-176">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ace89-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ace89-177">Request</span></span>

<span data-ttu-id="ace89-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ace89-178">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ace89-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="ace89-179">HTTP</span></span>](#tab/http)
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
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ace89-180">C#</span><span class="sxs-lookup"><span data-stu-id="ace89-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ace89-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ace89-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ace89-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ace89-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ace89-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="ace89-183">Response</span></span>

<span data-ttu-id="ace89-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ace89-184">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="ace89-185">Confira também</span><span class="sxs-lookup"><span data-stu-id="ace89-185">See also</span></span>

- [<span data-ttu-id="ace89-186">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="ace89-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ace89-187">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="ace89-187">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ace89-188">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="ace89-188">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
