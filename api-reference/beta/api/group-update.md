---
title: Atualizar grupo
description: Atualiza as propriedades de um objeto [Group](../resources/group.md) .
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e86835d13e2eda904b36ad0b77f9eeb3de57c1b2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869588"
---
# <a name="update-group"></a><span data-ttu-id="4b196-103">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="4b196-103">Update group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b196-104">Atualiza as propriedades de um objeto [Group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="4b196-104">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b196-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b196-105">Permissions</span></span>

<span data-ttu-id="4b196-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b196-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b196-108">Permission type</span></span>      | <span data-ttu-id="4b196-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b196-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b196-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b196-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b196-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b196-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="4b196-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b196-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b196-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b196-113">Not supported.</span></span>    |
|<span data-ttu-id="4b196-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b196-114">Application</span></span> | <span data-ttu-id="4b196-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b196-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b196-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b196-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4b196-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b196-117">Request headers</span></span>

| <span data-ttu-id="4b196-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4b196-118">Name</span></span>       | <span data-ttu-id="4b196-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b196-119">Type</span></span> | <span data-ttu-id="4b196-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b196-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4b196-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b196-121">Authorization</span></span>  | <span data-ttu-id="4b196-122">string</span><span class="sxs-lookup"><span data-stu-id="4b196-122">string</span></span>  | <span data-ttu-id="4b196-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b196-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b196-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b196-125">Request body</span></span>

<span data-ttu-id="4b196-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4b196-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b196-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b196-129">Property</span></span>   | <span data-ttu-id="4b196-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b196-130">Type</span></span> |<span data-ttu-id="4b196-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b196-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b196-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="4b196-132">allowExternalSenders</span></span>|<span data-ttu-id="4b196-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b196-133">Boolean</span></span>|<span data-ttu-id="4b196-p104">O padrão é **false**. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.</span><span class="sxs-lookup"><span data-stu-id="4b196-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="4b196-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="4b196-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="4b196-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b196-137">Boolean</span></span>|<span data-ttu-id="4b196-p105">O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="4b196-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="4b196-140">description</span><span class="sxs-lookup"><span data-stu-id="4b196-140">description</span></span>|<span data-ttu-id="4b196-141">String</span><span class="sxs-lookup"><span data-stu-id="4b196-141">String</span></span>|<span data-ttu-id="4b196-142">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="4b196-142">An optional description for the group.</span></span> |
|<span data-ttu-id="4b196-143">displayName</span><span class="sxs-lookup"><span data-stu-id="4b196-143">displayName</span></span>|<span data-ttu-id="4b196-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b196-144">String</span></span>|<span data-ttu-id="4b196-p106">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações.</span><span class="sxs-lookup"><span data-stu-id="4b196-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates.</span></span> |
|<span data-ttu-id="4b196-147">groupTypes</span><span class="sxs-lookup"><span data-stu-id="4b196-147">groupTypes</span></span>|<span data-ttu-id="4b196-148">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b196-148">String collection</span></span>|<span data-ttu-id="4b196-149">Especifica o tipo de grupo e sua associação.</span><span class="sxs-lookup"><span data-stu-id="4b196-149">Specifies the group type and its membership.</span></span>  <br><br><span data-ttu-id="4b196-150">Se a coleção contiver **Unificado** o grupo será um grupo do Office 365; caso contrário, será um grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="4b196-150">If the collection contains **Unified** then the group is an Office 365 group; otherwise it's a security group.</span></span>  <br><br><span data-ttu-id="4b196-151">Se a coleção incluir **DynamicMembership**, o grupo tem associação dinâmica; caso contrário, a associação é estática.</span><span class="sxs-lookup"><span data-stu-id="4b196-151">If the collection includes **DynamicMembership**, the group has dynamic membership; otherwise, membership is static.</span></span> |
|<span data-ttu-id="4b196-152">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="4b196-152">mailEnabled</span></span>|<span data-ttu-id="4b196-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b196-153">Boolean</span></span>|<span data-ttu-id="4b196-154">Especifica se o grupo está habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="4b196-154">Specifies whether the group is mail-enabled.</span></span> |
|<span data-ttu-id="4b196-155">mailNickname</span><span class="sxs-lookup"><span data-stu-id="4b196-155">mailNickname</span></span>|<span data-ttu-id="4b196-156">String</span><span class="sxs-lookup"><span data-stu-id="4b196-156">String</span></span>|<span data-ttu-id="4b196-157">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="4b196-157">The mail alias for the group.</span></span> <span data-ttu-id="4b196-158">Essa propriedade deve ser especificada quando um grupo é criado.</span><span class="sxs-lookup"><span data-stu-id="4b196-158">This property must be specified when a group is created.</span></span> |
|<span data-ttu-id="4b196-159">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="4b196-159">securityEnabled</span></span>|<span data-ttu-id="4b196-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b196-160">Boolean</span></span>|<span data-ttu-id="4b196-161">Especifica se o grupo é um grupo de segurança, incluindo grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4b196-161">Specifies whether the group is a security group, including Office 365 groups.</span></span> |
|<span data-ttu-id="4b196-162">visibility</span><span class="sxs-lookup"><span data-stu-id="4b196-162">visibility</span></span>|<span data-ttu-id="4b196-163">String</span><span class="sxs-lookup"><span data-stu-id="4b196-163">String</span></span>|<span data-ttu-id="4b196-p108">Especifica a visibilidade de um grupo do Office 365. Os valores possíveis são: **Private**, **Public** ou vazio (que é interpretado como **Public**).</span><span class="sxs-lookup"><span data-stu-id="4b196-p108">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="4b196-166">Como o recurso de **grupo** suporta [extensões](/graph/extensibility-overview), você pode usar `PATCH` a operação para adicionar, atualizar ou excluir seus próprios dados específicos de aplicativo em Propriedades personalizadas de uma extensão em uma instância de **grupo** existente.</span><span class="sxs-lookup"><span data-stu-id="4b196-166">Because the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>


> <span data-ttu-id="4b196-167">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="4b196-167">**Note:**</span></span>
>
> - <span data-ttu-id="4b196-168">Você pode atualizar o **autoSubscribeNewMembers** especificando-o em sua própria solicitação PATCH, sem incluir as demais propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="4b196-168">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="4b196-p109">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="4b196-p109">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>
> - <span data-ttu-id="4b196-172">As regras para atualizar os grupos de segurança habilitados para email no Microsoft Exchange Server podem ser complexas; Para saber mais, confira [Gerenciar grupos de segurança habilitados para email no Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span><span class="sxs-lookup"><span data-stu-id="4b196-172">The rules for updating mail-enabled security groups in Microsoft Exchange Server can be complex; to learn more, see [Manage mail-enabled security groups in Exchange Server](/Exchange/recipients/mail-enabled-security-groups?view=exchserver-2019).</span></span>



## <a name="response"></a><span data-ttu-id="4b196-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b196-173">Response</span></span>

<span data-ttu-id="4b196-174">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4b196-174">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4b196-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b196-175">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4b196-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b196-176">Request</span></span>

<span data-ttu-id="4b196-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b196-177">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4b196-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b196-178">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b196-179">C#</span><span class="sxs-lookup"><span data-stu-id="4b196-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b196-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b196-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b196-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b196-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4b196-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b196-182">Response</span></span>

<span data-ttu-id="4b196-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4b196-183">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="4b196-184">Confira também</span><span class="sxs-lookup"><span data-stu-id="4b196-184">See also</span></span>

- [<span data-ttu-id="4b196-185">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="4b196-185">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="4b196-186">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="4b196-186">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="4b196-187">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="4b196-187">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

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
