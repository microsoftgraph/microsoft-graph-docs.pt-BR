# <a name="create-group"></a><span data-ttu-id="80ea4-101">Criar grupo</span><span class="sxs-lookup"><span data-stu-id="80ea4-101">Create group</span></span>

<span data-ttu-id="80ea4-p101">Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:</span><span class="sxs-lookup"><span data-stu-id="80ea4-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="80ea4-104">Grupo do Office 365 (grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="80ea4-104">Office 365 group (unified group)</span></span>
* <span data-ttu-id="80ea4-105">Grupo dinâmico</span><span class="sxs-lookup"><span data-stu-id="80ea4-105">Dynamic group</span></span>
* <span data-ttu-id="80ea4-106">Grupo de segurança</span><span class="sxs-lookup"><span data-stu-id="80ea4-106">Security group</span></span>

> <span data-ttu-id="80ea4-p102">**Observação**: Embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="80ea4-p102">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80ea4-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80ea4-109">Prerequisites</span></span>
<span data-ttu-id="80ea4-110">O seguinte **escopo** é obrigatório para executar esta API: _Group.ReadWrite.All_</span><span class="sxs-lookup"><span data-stu-id="80ea4-110">The following **scope** is required to execute this API: _Group.ReadWrite.All_</span></span> 
## <a name="http-request"></a><span data-ttu-id="80ea4-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80ea4-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```
## <a name="request-headers"></a><span data-ttu-id="80ea4-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80ea4-112">Request headers</span></span>
| <span data-ttu-id="80ea4-113">Nome</span><span class="sxs-lookup"><span data-stu-id="80ea4-113">Name</span></span>       | <span data-ttu-id="80ea4-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="80ea4-114">Type</span></span> | <span data-ttu-id="80ea4-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ea4-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80ea4-116">Autorização</span><span class="sxs-lookup"><span data-stu-id="80ea4-116">Authorization</span></span>  | <span data-ttu-id="80ea4-117">string</span><span class="sxs-lookup"><span data-stu-id="80ea4-117">string</span></span>  | <span data-ttu-id="80ea4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80ea4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80ea4-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80ea4-120">Request body</span></span>
<span data-ttu-id="80ea4-121">A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar no mínimo quando cria um grupo.</span><span class="sxs-lookup"><span data-stu-id="80ea4-121">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="80ea4-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80ea4-122">Property</span></span> | <span data-ttu-id="80ea4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="80ea4-123">Type</span></span> | <span data-ttu-id="80ea4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ea4-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="80ea4-125">displayName</span><span class="sxs-lookup"><span data-stu-id="80ea4-125">displayName</span></span> | <span data-ttu-id="80ea4-126">string</span><span class="sxs-lookup"><span data-stu-id="80ea4-126">string</span></span> | <span data-ttu-id="80ea4-127">O nome de exibição no catálogo de endereços do grupo.</span><span class="sxs-lookup"><span data-stu-id="80ea4-127">The name to display in the address book for the group.</span></span> |
| <span data-ttu-id="80ea4-128">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="80ea4-128">mailEnabled</span></span> | <span data-ttu-id="80ea4-129">booliano</span><span class="sxs-lookup"><span data-stu-id="80ea4-129">boolean</span></span> | <span data-ttu-id="80ea4-p104">Defina como **true** para grupos habilitados para email. Defina isto como **false** se estiver criando um grupo do Office 365. Defina como **false** se estiver criando um grupo dinâmico ou de segurança.</span><span class="sxs-lookup"><span data-stu-id="80ea4-p104">Set to **true** for mail-enabled groups. Set this to **true** if creating an Office 365 group. Set this to **false** if creating dynamic or security group.</span></span>|
| <span data-ttu-id="80ea4-133">mailNickname</span><span class="sxs-lookup"><span data-stu-id="80ea4-133">mailNickname</span></span> | <span data-ttu-id="80ea4-134">string</span><span class="sxs-lookup"><span data-stu-id="80ea4-134">string</span></span> | <span data-ttu-id="80ea4-135">O alias de email do grupo.</span><span class="sxs-lookup"><span data-stu-id="80ea4-135">The mail alias for the group.</span></span> |
| <span data-ttu-id="80ea4-136">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="80ea4-136">securityEnabled</span></span> | <span data-ttu-id="80ea4-137">booliano</span><span class="sxs-lookup"><span data-stu-id="80ea4-137">boolean</span></span> | <span data-ttu-id="80ea4-p105">Defina como **true** para grupos de segurança. Definir isto como **true** se estiver criando um grupo dinâmico ou de segurança. Defina isto como **false** se estiver criando um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="80ea4-p105">Set to **true** for security-enabled groups. Set this to **true** if creating a dynamic or security group. Set this to **false** if creating an Office 365 group.</span></span> |

<span data-ttu-id="80ea4-141">Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.</span><span class="sxs-lookup"><span data-stu-id="80ea4-141">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="80ea4-142">Tipo de grupo</span><span class="sxs-lookup"><span data-stu-id="80ea4-142">Type of group</span></span> | <span data-ttu-id="80ea4-143">Propriedade **groupTypes**</span><span class="sxs-lookup"><span data-stu-id="80ea4-143">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="80ea4-144">Office 365 (também conhecido como grupo unificado)</span><span class="sxs-lookup"><span data-stu-id="80ea4-144">Office 365 (aka unified group)</span></span>| <span data-ttu-id="80ea4-145">"Unified"</span><span class="sxs-lookup"><span data-stu-id="80ea4-145">"Unified"</span></span> | 
| <span data-ttu-id="80ea4-146">Dinâmica</span><span class="sxs-lookup"><span data-stu-id="80ea4-146">Dynamic</span></span> | <span data-ttu-id="80ea4-147">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="80ea4-147">"DynamicMembership"</span></span> | 
| <span data-ttu-id="80ea4-148">Segurança</span><span class="sxs-lookup"><span data-stu-id="80ea4-148">Security</span></span> | <span data-ttu-id="80ea4-149">Não defina.</span><span class="sxs-lookup"><span data-stu-id="80ea4-149">Do not set.</span></span> | 

<span data-ttu-id="80ea4-p106">Especifique outras propriedades graváveis conforme necessário para o seu grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="80ea4-p106">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="80ea4-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ea4-152">Response</span></span>

<span data-ttu-id="80ea4-153">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [group](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80ea4-153">If successful, this method returns `201, Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80ea4-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80ea4-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80ea4-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80ea4-155">Request</span></span>
<span data-ttu-id="80ea4-156">Aqui está um exemplo de uma solicitação que cria um grupo do Office 365.</span><span class="sxs-lookup"><span data-stu-id="80ea4-156">Here is an example of a request that creates an Office 365 group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

##### <a name="response"></a><span data-ttu-id="80ea4-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ea4-157">Response</span></span>
<span data-ttu-id="80ea4-p107">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Mais propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80ea4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. More properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
