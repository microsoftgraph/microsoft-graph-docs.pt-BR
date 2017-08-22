# <a name="update-group"></a><span data-ttu-id="db259-101">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="db259-101">Update group</span></span>

<span data-ttu-id="db259-102">Atualizar as propriedades de um objeto group.</span><span class="sxs-lookup"><span data-stu-id="db259-102">Update the properties of a group object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db259-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db259-103">Prerequisites</span></span>
<span data-ttu-id="db259-104">O seguinte **escopo** é obrigatório para executar esta API: *Group.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="db259-104">The following **scope** is required to execute this API: *Group.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="db259-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db259-105">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db259-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db259-106">Request headers</span></span>

| <span data-ttu-id="db259-107">Nome</span><span class="sxs-lookup"><span data-stu-id="db259-107">Name</span></span>       | <span data-ttu-id="db259-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="db259-108">Type</span></span> | <span data-ttu-id="db259-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="db259-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db259-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="db259-110">Authorization</span></span>  | <span data-ttu-id="db259-111">string</span><span class="sxs-lookup"><span data-stu-id="db259-111">string</span></span>  | <span data-ttu-id="db259-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db259-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db259-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db259-114">Request body</span></span>

<span data-ttu-id="db259-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="db259-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="db259-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db259-118">Property</span></span>     | <span data-ttu-id="db259-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="db259-119">Type</span></span>   |<span data-ttu-id="db259-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="db259-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db259-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="db259-121">autoSubscribeNewMembers</span></span>|<span data-ttu-id="db259-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="db259-122">Boolean</span></span>|<span data-ttu-id="db259-p103">O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="db259-p103">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="db259-125">description</span><span class="sxs-lookup"><span data-stu-id="db259-125">description</span></span>|<span data-ttu-id="db259-126">String</span><span class="sxs-lookup"><span data-stu-id="db259-126">String</span></span>|<span data-ttu-id="db259-127">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="db259-127">An optional description for the group.</span></span> |
|<span data-ttu-id="db259-128">displayName</span><span class="sxs-lookup"><span data-stu-id="db259-128">displayName</span></span>|<span data-ttu-id="db259-129">String</span><span class="sxs-lookup"><span data-stu-id="db259-129">String</span></span>|<span data-ttu-id="db259-p104">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="db259-p104">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="db259-133">groupTypes</span><span class="sxs-lookup"><span data-stu-id="db259-133">groupTypes</span></span>|<span data-ttu-id="db259-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db259-134">String collection</span></span>|<span data-ttu-id="db259-p105">Especifica o tipo de grupo a ser criado. Os valores possíveis são **Unified** para criar um grupo do Office 365 ou **DynamicMembership** para grupos dinâmicos.  Para todos os outro tipos de grupos, como grupos habilitados para segurança e grupos de segurança habilitados para email, não defina essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="db259-p105">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="db259-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="db259-138">mailEnabled</span></span>|<span data-ttu-id="db259-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="db259-139">Boolean</span></span>|<span data-ttu-id="db259-p106">Especifica se o grupo está habilitado para email. Se a propriedade **securityEnabled** também é **true**, o grupo é um grupo de segurança habilitado para email. Caso contrário, o grupo é um grupo de distribuição do Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="db259-p106">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="db259-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="db259-142">mailNickname</span></span>|<span data-ttu-id="db259-143">String</span><span class="sxs-lookup"><span data-stu-id="db259-143">String</span></span>|<span data-ttu-id="db259-p107">O alias de email do grupo. Essa propriedade deve ser especificada quando um grupo é criado. Dá suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="db259-p107">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="db259-147">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="db259-147">securityEnabled</span></span>|<span data-ttu-id="db259-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="db259-148">Boolean</span></span>|<span data-ttu-id="db259-p108">Especifica se o grupo é um grupo de segurança. Se a propriedade **mailEnabled** também é true, o grupo é um grupo de segurança habilitado para email; caso contrário, é um grupo de segurança. Deve ser **false** para grupos do Office 365. Dá suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="db259-p108">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="db259-153">visibilidade</span><span class="sxs-lookup"><span data-stu-id="db259-153">visibility</span></span>|<span data-ttu-id="db259-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="db259-154">Boolean</span></span>|<span data-ttu-id="db259-p109">Especifica a visibilidade de um grupo do Office 365. Os valores possíveis são: **Private**, **Public** ou vazio (que é interpretado como **Public**).</span><span class="sxs-lookup"><span data-stu-id="db259-p109">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="db259-157">**Observação**</span><span class="sxs-lookup"><span data-stu-id="db259-157">**Note**</span></span>

- <span data-ttu-id="db259-158">Você pode atualizar o **autoSubscribeNewMembers** especificando-o em sua própria solicitação PATCH, sem incluir as demais propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="db259-158">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="db259-p110">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="db259-p110">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="db259-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="db259-162">Response</span></span>

<span data-ttu-id="db259-163">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="db259-163">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="db259-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db259-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="db259-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db259-165">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="db259-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="db259-166">Response</span></span>

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