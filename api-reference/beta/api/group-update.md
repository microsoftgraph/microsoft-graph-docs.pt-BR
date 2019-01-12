---
title: Atualizar grupo
description: Atualizar as propriedades de um objeto group.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f1f86067771a4732c8839f48bc02dd3edd15c19b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915232"
---
# <a name="update-group"></a><span data-ttu-id="92fc8-103">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="92fc8-103">Update group</span></span>

> <span data-ttu-id="92fc8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="92fc8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92fc8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="92fc8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="92fc8-106">Atualize as propriedades de um objeto [group](../resources/group.md) .</span><span class="sxs-lookup"><span data-stu-id="92fc8-106">Update the properties of a [group](../resources/group.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="92fc8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="92fc8-107">Permissions</span></span>

<span data-ttu-id="92fc8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92fc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92fc8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92fc8-110">Permission type</span></span>      | <span data-ttu-id="92fc8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92fc8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92fc8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92fc8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="92fc8-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92fc8-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="92fc8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92fc8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92fc8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92fc8-115">Not supported.</span></span>    |
|<span data-ttu-id="92fc8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92fc8-116">Application</span></span> | <span data-ttu-id="92fc8-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92fc8-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92fc8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92fc8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92fc8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92fc8-119">Request headers</span></span>

| <span data-ttu-id="92fc8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="92fc8-120">Name</span></span>       | <span data-ttu-id="92fc8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="92fc8-121">Type</span></span> | <span data-ttu-id="92fc8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="92fc8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="92fc8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92fc8-123">Authorization</span></span>  | <span data-ttu-id="92fc8-124">string</span><span class="sxs-lookup"><span data-stu-id="92fc8-124">string</span></span>  | <span data-ttu-id="92fc8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92fc8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92fc8-127">Request body</span></span>

<span data-ttu-id="92fc8-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="92fc8-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92fc8-131">Property</span></span>   | <span data-ttu-id="92fc8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="92fc8-132">Type</span></span> |<span data-ttu-id="92fc8-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="92fc8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92fc8-134">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="92fc8-134">allowExternalSenders</span></span>|<span data-ttu-id="92fc8-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="92fc8-135">Boolean</span></span>|<span data-ttu-id="92fc8-p105">O padrão é **false**. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p105">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="92fc8-138">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="92fc8-138">autoSubscribeNewMembers</span></span>|<span data-ttu-id="92fc8-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="92fc8-139">Boolean</span></span>|<span data-ttu-id="92fc8-p106">O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p106">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="92fc8-142">description</span><span class="sxs-lookup"><span data-stu-id="92fc8-142">description</span></span>|<span data-ttu-id="92fc8-143">String</span><span class="sxs-lookup"><span data-stu-id="92fc8-143">String</span></span>|<span data-ttu-id="92fc8-144">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="92fc8-144">An optional description for the group.</span></span> |
|<span data-ttu-id="92fc8-145">displayName</span><span class="sxs-lookup"><span data-stu-id="92fc8-145">displayName</span></span>|<span data-ttu-id="92fc8-146">String</span><span class="sxs-lookup"><span data-stu-id="92fc8-146">String</span></span>|<span data-ttu-id="92fc8-p107">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p107">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="92fc8-150">groupTypes</span><span class="sxs-lookup"><span data-stu-id="92fc8-150">groupTypes</span></span>|<span data-ttu-id="92fc8-151">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="92fc8-151">String collection</span></span>|<span data-ttu-id="92fc8-p108">Especifica o tipo de grupo a ser criado. Os valores possíveis são **Unified** para criar um grupo do Office 365 ou **DynamicMembership** para grupos dinâmicos.  Para todos os outro tipos de grupos, como grupos habilitados para segurança e grupos de segurança habilitados para email, não defina essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p108">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="92fc8-155">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="92fc8-155">mailEnabled</span></span>|<span data-ttu-id="92fc8-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="92fc8-156">Boolean</span></span>|<span data-ttu-id="92fc8-p109">Especifica se o grupo está habilitado para email. Se a propriedade **securityEnabled** também é **true**, o grupo é um grupo de segurança habilitado para email. Caso contrário, o grupo é um grupo de distribuição do Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p109">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="92fc8-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="92fc8-159">mailNickname</span></span>|<span data-ttu-id="92fc8-160">String</span><span class="sxs-lookup"><span data-stu-id="92fc8-160">String</span></span>|<span data-ttu-id="92fc8-p110">O alias de email do grupo. Essa propriedade deve ser especificada quando um grupo é criado. Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p110">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="92fc8-164">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="92fc8-164">securityEnabled</span></span>|<span data-ttu-id="92fc8-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="92fc8-165">Boolean</span></span>|<span data-ttu-id="92fc8-p111">Especifica se o grupo é um grupo de segurança. Se a propriedade **mailEnabled** também é true, o grupo é um grupo de segurança habilitado para email; caso contrário, é um grupo de segurança. Deve ser **false** para grupos do Office 365. Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="92fc8-p111">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="92fc8-170">visibilidade</span><span class="sxs-lookup"><span data-stu-id="92fc8-170">visibility</span></span>|<span data-ttu-id="92fc8-171">String</span><span class="sxs-lookup"><span data-stu-id="92fc8-171">String</span></span>|<span data-ttu-id="92fc8-p112">Especifica a visibilidade de um grupo do Office 365. Os valores possíveis são: **Private**, **Public** ou vazio (que é interpretado como **Public**).</span><span class="sxs-lookup"><span data-stu-id="92fc8-p112">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="92fc8-174">Desde que o recurso de **grupo** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância existente do **grupo** .</span><span class="sxs-lookup"><span data-stu-id="92fc8-174">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **group** instance.</span></span>

> <span data-ttu-id="92fc8-175">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="92fc8-175">**Note:**</span></span>
>
> - <span data-ttu-id="92fc8-176">Você pode atualizar o **autoSubscribeNewMembers** especificando-o em sua própria solicitação PATCH, sem incluir as demais propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="92fc8-176">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
> - <span data-ttu-id="92fc8-p113">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="92fc8-p113">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="92fc8-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="92fc8-180">Response</span></span>

<span data-ttu-id="92fc8-181">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="92fc8-181">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="92fc8-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92fc8-182">Example</span></span>

#### <a name="request"></a><span data-ttu-id="92fc8-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92fc8-183">Request</span></span>

<span data-ttu-id="92fc8-184">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92fc8-184">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="92fc8-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="92fc8-185">Response</span></span>

<span data-ttu-id="92fc8-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92fc8-186">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="92fc8-187">Confira também</span><span class="sxs-lookup"><span data-stu-id="92fc8-187">See also</span></span>

- [<span data-ttu-id="92fc8-188">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="92fc8-188">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="92fc8-189">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="92fc8-189">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="92fc8-190">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="92fc8-190">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
