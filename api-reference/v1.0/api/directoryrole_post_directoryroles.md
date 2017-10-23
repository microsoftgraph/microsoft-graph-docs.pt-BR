# <a name="activate-directoryrole"></a><span data-ttu-id="a7a61-101">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="a7a61-101">Activate directoryRole</span></span>

<span data-ttu-id="a7a61-p101">Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="a7a61-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="a7a61-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a7a61-106">Permissions</span></span>
<span data-ttu-id="a7a61-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7a61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a7a61-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7a61-109">Permission type</span></span>      | <span data-ttu-id="a7a61-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a7a61-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7a61-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7a61-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7a61-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7a61-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a7a61-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7a61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7a61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7a61-114">Not supported.</span></span>    |
|<span data-ttu-id="a7a61-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7a61-115">Application</span></span> | <span data-ttu-id="a7a61-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7a61-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7a61-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7a61-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="a7a61-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7a61-118">Request headers</span></span>
| <span data-ttu-id="a7a61-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a7a61-119">Name</span></span>       | <span data-ttu-id="a7a61-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7a61-120">Type</span></span> | <span data-ttu-id="a7a61-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7a61-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a7a61-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7a61-122">Authorization</span></span>  | <span data-ttu-id="a7a61-123">string</span><span class="sxs-lookup"><span data-stu-id="a7a61-123">string</span></span>  | <span data-ttu-id="a7a61-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7a61-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7a61-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7a61-126">Content-Type</span></span>  | <span data-ttu-id="a7a61-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a7a61-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7a61-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7a61-128">Request body</span></span>
<span data-ttu-id="a7a61-129">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="a7a61-129">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="a7a61-130">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="a7a61-130">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="a7a61-131">Parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="a7a61-131">Required parameter</span></span> | <span data-ttu-id="a7a61-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7a61-132">Type</span></span> | <span data-ttu-id="a7a61-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7a61-133">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="a7a61-134">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="a7a61-134">roleTemplateId</span></span> | <span data-ttu-id="a7a61-135">string</span><span class="sxs-lookup"><span data-stu-id="a7a61-135">string</span></span> | <span data-ttu-id="a7a61-p104">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7a61-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="a7a61-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7a61-138">Response</span></span>

<span data-ttu-id="a7a61-139">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7a61-139">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7a61-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7a61-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7a61-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7a61-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="a7a61-142">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="a7a61-142">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a7a61-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7a61-143">Response</span></span>
<span data-ttu-id="a7a61-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7a61-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
