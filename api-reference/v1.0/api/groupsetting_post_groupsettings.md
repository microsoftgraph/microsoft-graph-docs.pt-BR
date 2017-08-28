# <a name="create-a-group-setting"></a><span data-ttu-id="b57df-101">Criar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="b57df-101">Create a group setting</span></span>

<span data-ttu-id="b57df-p101">Use essa API para criar uma nova configuração com base nos modelos disponíveis em [groupSettingTemplates](../resources/groupsettingtemplate.md). Essas configurações podem ser no nível do locatário ou do grupo. A solicitação de criação precisa fornecer [settingValues](../resources/settingvalue.md) para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que rege se os membros de um grupo podem convidar usuários convidados pode ser definida. Isso controlará esse comportamento depois que a capacidade de adicionar usuários convidados a um grupo esteja disponível de forma geral.</span><span class="sxs-lookup"><span data-stu-id="b57df-p101">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

## <a name="permissions"></a><span data-ttu-id="b57df-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b57df-107">Permissions</span></span>

<span data-ttu-id="b57df-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b57df-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="b57df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b57df-110">Permission type</span></span>      | <span data-ttu-id="b57df-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b57df-111">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="b57df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b57df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b57df-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b57df-113">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="b57df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b57df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b57df-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b57df-115">Not supported.</span></span>    | 
|<span data-ttu-id="b57df-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b57df-116">Application</span></span> | <span data-ttu-id="b57df-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b57df-117">Directory.ReadWrite.All</span></span> | 


## <a name="http-request"></a><span data-ttu-id="b57df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b57df-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="b57df-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b57df-119">Request headers</span></span>

| <span data-ttu-id="b57df-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b57df-120">Name</span></span> | <span data-ttu-id="b57df-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b57df-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b57df-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b57df-122">Authorization</span></span> | <span data-ttu-id="b57df-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b57df-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b57df-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b57df-125">Content-Type</span></span> | <span data-ttu-id="b57df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b57df-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b57df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b57df-127">Request body</span></span>
<span data-ttu-id="b57df-p104">No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md). No entanto, o nome de exibição para que a configuração será definida com base no nome do modelo configurações referenciado.</span><span class="sxs-lookup"><span data-stu-id="b57df-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="b57df-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b57df-130">Response</span></span>

<span data-ttu-id="b57df-131">Se bem-sucedido, este método retorna o código de resposta `201, Created` e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b57df-131">If successful, this method returns `201, Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b57df-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b57df-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b57df-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b57df-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "groupSetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="b57df-134">No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md).</span><span class="sxs-lookup"><span data-stu-id="b57df-134">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b57df-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b57df-135">Response</span></span>

<span data-ttu-id="b57df-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b57df-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "groupSetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ],
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->