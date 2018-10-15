# <a name="activate-directoryrole"></a><span data-ttu-id="2f11d-101">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="2f11d-101">Activate directoryRole</span></span>

<span data-ttu-id="2f11d-p101">Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="2f11d-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f11d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f11d-106">Permissions</span></span>
<span data-ttu-id="2f11d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f11d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2f11d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f11d-109">Permission type</span></span>      | <span data-ttu-id="2f11d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f11d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f11d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f11d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2f11d-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f11d-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2f11d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f11d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f11d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f11d-114">Not supported.</span></span>    |
|<span data-ttu-id="2f11d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f11d-115">Application</span></span> | <span data-ttu-id="2f11d-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f11d-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f11d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f11d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="2f11d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f11d-118">Request headers</span></span>
| <span data-ttu-id="2f11d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2f11d-119">Name</span></span>       | <span data-ttu-id="2f11d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f11d-120">Type</span></span> | <span data-ttu-id="2f11d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f11d-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f11d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f11d-122">Authorization</span></span>  | <span data-ttu-id="2f11d-123">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f11d-123">string</span></span>  | <span data-ttu-id="2f11d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f11d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f11d-126">Conteúdo-Tipo</span><span class="sxs-lookup"><span data-stu-id="2f11d-126">Content-Type</span></span>  | <span data-ttu-id="2f11d-127">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f11d-127">string</span></span>  | <span data-ttu-id="2f11d-128">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="2f11d-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f11d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f11d-129">Request body</span></span>
<span data-ttu-id="2f11d-130">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="2f11d-130">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="2f11d-131">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="2f11d-131">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="2f11d-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2f11d-132">Parameter</span></span> | <span data-ttu-id="2f11d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f11d-133">Type</span></span> | <span data-ttu-id="2f11d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f11d-134">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="2f11d-135">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="2f11d-135">roleTemplateId</span></span> | <span data-ttu-id="2f11d-136">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f11d-136">string</span></span> | <span data-ttu-id="2f11d-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f11d-137">Required.</span></span> <span data-ttu-id="2f11d-138">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função é baseada.</span><span class="sxs-lookup"><span data-stu-id="2f11d-138">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span> <span data-ttu-id="2f11d-139">Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f11d-139">The ID of the directoryRoleTemplate that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="2f11d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f11d-140">Response</span></span>

<span data-ttu-id="2f11d-141">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f11d-141">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f11d-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f11d-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f11d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f11d-143">Request</span></span>

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
<span data-ttu-id="2f11d-144">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="2f11d-144">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2f11d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f11d-145">Response</span></span>
<span data-ttu-id="2f11d-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f11d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
