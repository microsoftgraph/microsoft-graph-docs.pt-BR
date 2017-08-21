# <a name="activate-directoryrole"></a><span data-ttu-id="34523-101">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="34523-101">Activate directoryRole</span></span>

<span data-ttu-id="34523-p101">Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente Administradores de Empresa e as funções de Usuários de diretório implícitas são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="34523-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34523-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34523-106">Prerequisites</span></span>
<span data-ttu-id="34523-107">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="34523-107">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="34523-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34523-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="34523-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34523-109">Request headers</span></span>
| <span data-ttu-id="34523-110">Nome</span><span class="sxs-lookup"><span data-stu-id="34523-110">Name</span></span>       | <span data-ttu-id="34523-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="34523-111">Type</span></span> | <span data-ttu-id="34523-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="34523-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34523-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="34523-113">Authorization</span></span>  | <span data-ttu-id="34523-114">string</span><span class="sxs-lookup"><span data-stu-id="34523-114">string</span></span>  | <span data-ttu-id="34523-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34523-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34523-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34523-117">Content-Type</span></span>  | <span data-ttu-id="34523-118">application/json</span><span class="sxs-lookup"><span data-stu-id="34523-118">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34523-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34523-119">Request body</span></span>
<span data-ttu-id="34523-120">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="34523-120">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="34523-121">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="34523-121">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="34523-122">Parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="34523-122">Required parameter</span></span> | <span data-ttu-id="34523-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="34523-123">Type</span></span> | <span data-ttu-id="34523-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="34523-124">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="34523-125">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="34523-125">roleTemplateId</span></span> | <span data-ttu-id="34523-126">string</span><span class="sxs-lookup"><span data-stu-id="34523-126">string</span></span> | <span data-ttu-id="34523-p103">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="34523-p103">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="34523-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34523-129">Response</span></span>

<span data-ttu-id="34523-130">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34523-130">If successful, this method returns `201, Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34523-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34523-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34523-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34523-132">Request</span></span>

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
<span data-ttu-id="34523-133">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="34523-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="34523-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="34523-134">Response</span></span>
<span data-ttu-id="34523-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34523-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
