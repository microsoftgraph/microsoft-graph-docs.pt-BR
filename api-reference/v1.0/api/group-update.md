---
title: Atualizar grupo
description: Atualizar as propriedades de um objeto group.
author: dkershaw10
ms.openlocfilehash: 11144b477d6a19ae876eed1f561ade4a139564a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347401"
---
# <a name="update-group"></a><span data-ttu-id="1352b-103">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="1352b-103">Update group</span></span>

<span data-ttu-id="1352b-104">Atualizar as propriedades de um objeto group.</span><span class="sxs-lookup"><span data-stu-id="1352b-104">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1352b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1352b-105">Permissions</span></span>

<span data-ttu-id="1352b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1352b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1352b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1352b-108">Permission type</span></span>      | <span data-ttu-id="1352b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1352b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1352b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1352b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1352b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1352b-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1352b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1352b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1352b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1352b-113">Not supported.</span></span>    |
|<span data-ttu-id="1352b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1352b-114">Application</span></span> | <span data-ttu-id="1352b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1352b-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1352b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1352b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1352b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1352b-117">Request headers</span></span>

| <span data-ttu-id="1352b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1352b-118">Name</span></span>       | <span data-ttu-id="1352b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1352b-119">Type</span></span> | <span data-ttu-id="1352b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1352b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1352b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1352b-121">Authorization</span></span>  | <span data-ttu-id="1352b-122">string</span><span class="sxs-lookup"><span data-stu-id="1352b-122">string</span></span>  | <span data-ttu-id="1352b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1352b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1352b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1352b-125">Request body</span></span>

<span data-ttu-id="1352b-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1352b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1352b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1352b-129">Property</span></span>   | <span data-ttu-id="1352b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1352b-130">Type</span></span> |<span data-ttu-id="1352b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1352b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1352b-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="1352b-132">allowExternalSenders</span></span>|<span data-ttu-id="1352b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="1352b-133">Boolean</span></span>|<span data-ttu-id="1352b-p104">O padrão é **false**. Indica se as pessoas externas à empresa podem enviar mensagens para o grupo.</span><span class="sxs-lookup"><span data-stu-id="1352b-p104">Default is **false**. Indicates if people external to the organization can send messages to the group.</span></span>|
|<span data-ttu-id="1352b-136">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="1352b-136">autoSubscribeNewMembers</span></span>|<span data-ttu-id="1352b-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1352b-137">Boolean</span></span>|<span data-ttu-id="1352b-p105">O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="1352b-p105">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="1352b-140">description</span><span class="sxs-lookup"><span data-stu-id="1352b-140">description</span></span>|<span data-ttu-id="1352b-141">String</span><span class="sxs-lookup"><span data-stu-id="1352b-141">String</span></span>|<span data-ttu-id="1352b-142">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="1352b-142">An optional description for the group.</span></span> |
|<span data-ttu-id="1352b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="1352b-143">displayName</span></span>|<span data-ttu-id="1352b-144">String</span><span class="sxs-lookup"><span data-stu-id="1352b-144">String</span></span>|<span data-ttu-id="1352b-p106">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="1352b-p106">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="1352b-148">groupTypes</span><span class="sxs-lookup"><span data-stu-id="1352b-148">groupTypes</span></span>|<span data-ttu-id="1352b-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1352b-149">String collection</span></span>|<span data-ttu-id="1352b-p107">Especifica o tipo de grupo a ser criado. Os valores possíveis são **Unified** para criar um grupo do Office 365 ou **DynamicMembership** para grupos dinâmicos.  Para todos os outro tipos de grupos, como grupos habilitados para segurança e grupos de segurança habilitados para email, não defina essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="1352b-p107">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="1352b-153">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="1352b-153">mailEnabled</span></span>|<span data-ttu-id="1352b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="1352b-154">Boolean</span></span>|<span data-ttu-id="1352b-p108">Especifica se o grupo está habilitado para email. Se a propriedade **securityEnabled** também é **true**, o grupo é um grupo de segurança habilitado para email. Caso contrário, o grupo é um grupo de distribuição do Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="1352b-p108">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="1352b-157">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1352b-157">mailNickname</span></span>|<span data-ttu-id="1352b-158">String</span><span class="sxs-lookup"><span data-stu-id="1352b-158">String</span></span>|<span data-ttu-id="1352b-p109">O alias de email do grupo. Essa propriedade deve ser especificada quando um grupo é criado. Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="1352b-p109">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="1352b-162">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="1352b-162">securityEnabled</span></span>|<span data-ttu-id="1352b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="1352b-163">Boolean</span></span>|<span data-ttu-id="1352b-p110">Especifica se o grupo é um grupo de segurança. Se a propriedade **mailEnabled** também é true, o grupo é um grupo de segurança habilitado para email; caso contrário, é um grupo de segurança. Deve ser **false** para grupos do Office 365. Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="1352b-p110">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="1352b-168">visibilidade</span><span class="sxs-lookup"><span data-stu-id="1352b-168">visibility</span></span>|<span data-ttu-id="1352b-169">String</span><span class="sxs-lookup"><span data-stu-id="1352b-169">String</span></span>|<span data-ttu-id="1352b-170">Especifica a visibilidade de um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1352b-170">Specifies the visibility of an Office 365 group.</span></span> <span data-ttu-id="1352b-171">Os valores possíveis são: **particular**, **público**ou em branco (que será interpretado como **pública**).</span><span class="sxs-lookup"><span data-stu-id="1352b-171">The possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

> <span data-ttu-id="1352b-172">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="1352b-172">**Note:**</span></span>
>
> - <span data-ttu-id="1352b-173">Você pode atualizar **autoSubscribeNewMembers** especificando-o no seu próprio solicitação de PATCH, sem incluir as outras propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="1352b-173">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request,without including the other properties in the table above.</span></span>
> - <span data-ttu-id="1352b-p112">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="1352b-p112">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="1352b-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="1352b-177">Response</span></span>

<span data-ttu-id="1352b-178">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1352b-178">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1352b-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1352b-179">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1352b-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1352b-180">Request</span></span>

<span data-ttu-id="1352b-181">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1352b-181">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="1352b-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="1352b-182">Response</span></span>

<span data-ttu-id="1352b-183">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1352b-183">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->