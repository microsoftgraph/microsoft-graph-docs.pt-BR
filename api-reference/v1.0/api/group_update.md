# <a name="update-group"></a><span data-ttu-id="1aedd-101">Atualizar grupo</span><span class="sxs-lookup"><span data-stu-id="1aedd-101">Update group</span></span>

<span data-ttu-id="1aedd-102">Atualizar as propriedades de um objeto group.</span><span class="sxs-lookup"><span data-stu-id="1aedd-102">Update the properties of a group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1aedd-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="1aedd-103">Permissions</span></span>
<span data-ttu-id="1aedd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1aedd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="1aedd-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1aedd-106">Permission type</span></span>      | <span data-ttu-id="1aedd-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1aedd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1aedd-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1aedd-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1aedd-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aedd-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1aedd-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1aedd-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1aedd-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1aedd-111">Not supported.</span></span>    |
|<span data-ttu-id="1aedd-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1aedd-112">Application</span></span> | <span data-ttu-id="1aedd-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1aedd-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1aedd-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1aedd-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1aedd-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1aedd-115">Request headers</span></span>

| <span data-ttu-id="1aedd-116">Nome</span><span class="sxs-lookup"><span data-stu-id="1aedd-116">Name</span></span>       | <span data-ttu-id="1aedd-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aedd-117">Type</span></span> | <span data-ttu-id="1aedd-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aedd-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1aedd-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="1aedd-119">Authorization</span></span>  | <span data-ttu-id="1aedd-120">string</span><span class="sxs-lookup"><span data-stu-id="1aedd-120">string</span></span>  | <span data-ttu-id="1aedd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1aedd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1aedd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1aedd-123">Request body</span></span>

<span data-ttu-id="1aedd-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1aedd-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1aedd-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1aedd-127">Property</span></span>     | <span data-ttu-id="1aedd-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="1aedd-128">Type</span></span>   |<span data-ttu-id="1aedd-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="1aedd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1aedd-130">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="1aedd-130">autoSubscribeNewMembers</span></span>|<span data-ttu-id="1aedd-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aedd-131">Boolean</span></span>|<span data-ttu-id="1aedd-p104">O padrão é **false**. Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email.</span><span class="sxs-lookup"><span data-stu-id="1aedd-p104">Default is **false**. Indicates if new members added to the group will be auto-subscribed to receive email notifications.</span></span>|
|<span data-ttu-id="1aedd-134">descrição</span><span class="sxs-lookup"><span data-stu-id="1aedd-134">description</span></span>|<span data-ttu-id="1aedd-135">String</span><span class="sxs-lookup"><span data-stu-id="1aedd-135">String</span></span>|<span data-ttu-id="1aedd-136">Uma descrição opcional para o grupo.</span><span class="sxs-lookup"><span data-stu-id="1aedd-136">An optional description for the group.</span></span> |
|<span data-ttu-id="1aedd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1aedd-137">displayName</span></span>|<span data-ttu-id="1aedd-138">String</span><span class="sxs-lookup"><span data-stu-id="1aedd-138">String</span></span>|<span data-ttu-id="1aedd-p105">O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.</span><span class="sxs-lookup"><span data-stu-id="1aedd-p105">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="1aedd-142">groupTypes</span><span class="sxs-lookup"><span data-stu-id="1aedd-142">groupTypes</span></span>|<span data-ttu-id="1aedd-143">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1aedd-143">String collection</span></span>|<span data-ttu-id="1aedd-p106">Especifica o tipo de grupo a ser criado. Os valores possíveis são **Unified** para criar um grupo do Office 365 ou **DynamicMembership** para grupos dinâmicos.  Para todos os outro tipos de grupos, como grupos habilitados para segurança e grupos de segurança habilitados para email, não defina essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="1aedd-p106">Specifies the type of group to create. Possible values are **Unified** to create an Office 365 group, or **DynamicMembership** for dynamic groups.  For all other group types, like security-enabled groups and email-enabled security groups, do not set this property.</span></span>|
|<span data-ttu-id="1aedd-147">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="1aedd-147">mailEnabled</span></span>|<span data-ttu-id="1aedd-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aedd-148">Boolean</span></span>|<span data-ttu-id="1aedd-p107">Especifica se o grupo está habilitado para email. Se a propriedade **securityEnabled** também é **true**, o grupo é um grupo de segurança habilitado para email. Caso contrário, o grupo é um grupo de distribuição do Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="1aedd-p107">Specifies whether the group is mail-enabled. If the **securityEnabled** property is also **true**, the group is a mail-enabled security group; otherwise, the group is a Microsoft Exchange distribution group.</span></span>|
|<span data-ttu-id="1aedd-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1aedd-151">mailNickname</span></span>|<span data-ttu-id="1aedd-152">String</span><span class="sxs-lookup"><span data-stu-id="1aedd-152">String</span></span>|<span data-ttu-id="1aedd-p108">O alias de email do grupo. Essa propriedade deve ser especificada quando um grupo é criado. Dá suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="1aedd-p108">The mail alias for the group. This property must be specified when a group is created. Supports $filter.</span></span>|
|<span data-ttu-id="1aedd-156">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="1aedd-156">securityEnabled</span></span>|<span data-ttu-id="1aedd-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aedd-157">Boolean</span></span>|<span data-ttu-id="1aedd-p109">Especifica se o grupo é um grupo de segurança. Se a propriedade **mailEnabled** também é true, o grupo é um grupo de segurança habilitado para email; caso contrário, é um grupo de segurança. Deve ser **false** para grupos do Office 365. Dá suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="1aedd-p109">Specifies whether the group is a security group. If the **mailEnabled** property is also true, the group is a mail-enabled security group; otherwise it is a security group. Must be **false** for Office 365 groups. Supports $filter..</span></span>|
|<span data-ttu-id="1aedd-162">visibilidade</span><span class="sxs-lookup"><span data-stu-id="1aedd-162">visibility</span></span>|<span data-ttu-id="1aedd-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="1aedd-163">Boolean</span></span>|<span data-ttu-id="1aedd-p110">Especifica a visibilidade de um grupo do Office 365. Os valores possíveis são: **Private**, **Public** ou vazio (que é interpretado como **Public**).</span><span class="sxs-lookup"><span data-stu-id="1aedd-p110">Specifies the visibility of an Office 365 group. Possible values are: **Private**, **Public**, or empty (which is interpreted as **Public**).</span></span>|

<span data-ttu-id="1aedd-166">**Observação**</span><span class="sxs-lookup"><span data-stu-id="1aedd-166">**Note**</span></span>

- <span data-ttu-id="1aedd-167">Você pode atualizar o **autoSubscribeNewMembers** especificando-o em sua própria solicitação PATCH, sem incluir as demais propriedades na tabela acima.</span><span class="sxs-lookup"><span data-stu-id="1aedd-167">You can update **autoSubscribeNewMembers** by specifying it in its own PATCH request, without including the other properties in the table above.</span></span>
- <span data-ttu-id="1aedd-p111">Apenas um subconjunto da API de grupo relacionado à administração do grupo principal e ao aplicativo de suporte para gerenciamento às permissões delegadas. Todos os outros membros da API do grupo, inclusive a atualização **autoSubscribeNewMembers**, dão suporte apenas a permissões delegadas. Confira exemplos nos [problemas conhecidos](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes).</span><span class="sxs-lookup"><span data-stu-id="1aedd-p111">Only a subset of the group API pertaining to core group administration and management support application and delegated permissions. All other members of the group API, including updating  **autoSubscribeNewMembers**, support only delegated permissions. See [known issues](https://developer.microsoft.com/en-us/graph/docs/overview/release_notes#group-permission-scopes) for examples.</span></span>

## <a name="response"></a><span data-ttu-id="1aedd-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aedd-171">Response</span></span>

<span data-ttu-id="1aedd-172">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1aedd-172">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1aedd-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1aedd-173">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1aedd-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1aedd-174">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="1aedd-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="1aedd-175">Response</span></span>

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