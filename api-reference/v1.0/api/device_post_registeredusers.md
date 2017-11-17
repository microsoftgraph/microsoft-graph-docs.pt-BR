# <a name="create-registereduser"></a><span data-ttu-id="e6015-101">Criar registeredUser</span><span class="sxs-lookup"><span data-stu-id="e6015-101">Create registeredUser</span></span>

<span data-ttu-id="e6015-102">Adiciona um usuário registrado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e6015-102">Add a registered user for the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6015-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6015-103">Permissions</span></span>
<span data-ttu-id="e6015-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6015-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e6015-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6015-106">Permission type</span></span>      | <span data-ttu-id="e6015-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6015-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6015-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6015-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e6015-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6015-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6015-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6015-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6015-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6015-111">Not supported.</span></span>    |
|<span data-ttu-id="e6015-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6015-112">Application</span></span> | <span data-ttu-id="e6015-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6015-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6015-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6015-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers

```
## <a name="request-headers"></a><span data-ttu-id="e6015-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6015-115">Request headers</span></span>
| <span data-ttu-id="e6015-116">Nome</span><span class="sxs-lookup"><span data-stu-id="e6015-116">Name</span></span>       | <span data-ttu-id="e6015-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6015-117">Type</span></span> | <span data-ttu-id="e6015-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6015-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e6015-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6015-119">Authorization</span></span>  | <span data-ttu-id="e6015-120">string</span><span class="sxs-lookup"><span data-stu-id="e6015-120">string</span></span>  | <span data-ttu-id="e6015-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6015-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6015-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6015-123">Request body</span></span>
<span data-ttu-id="e6015-124">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e6015-124">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e6015-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6015-125">Response</span></span>

<span data-ttu-id="e6015-126">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6015-126">If successful, this method returns `201 Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6015-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6015-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6015-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6015-128">Request</span></span>
<span data-ttu-id="e6015-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6015-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="e6015-130">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e6015-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e6015-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6015-131">Response</span></span>
<span data-ttu-id="e6015-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6015-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 51

{
  "directoryObject": {
    "id": "id-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create registeredUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->