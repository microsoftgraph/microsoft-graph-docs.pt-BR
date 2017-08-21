# <a name="create-registereduser"></a><span data-ttu-id="f46d5-101">Criar registeredUser</span><span class="sxs-lookup"><span data-stu-id="f46d5-101">Create registeredUser</span></span>

<span data-ttu-id="f46d5-102">Adiciona um usuário registrado ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f46d5-102">Add a registered user for the device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f46d5-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f46d5-103">Prerequisites</span></span>
<span data-ttu-id="f46d5-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="f46d5-104">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="f46d5-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f46d5-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredUsers

```
## <a name="request-headers"></a><span data-ttu-id="f46d5-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f46d5-106">Request headers</span></span>
| <span data-ttu-id="f46d5-107">Nome</span><span class="sxs-lookup"><span data-stu-id="f46d5-107">Name</span></span>       | <span data-ttu-id="f46d5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f46d5-108">Type</span></span> | <span data-ttu-id="f46d5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f46d5-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f46d5-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="f46d5-110">Authorization</span></span>  | <span data-ttu-id="f46d5-111">string</span><span class="sxs-lookup"><span data-stu-id="f46d5-111">string</span></span>  | <span data-ttu-id="f46d5-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f46d5-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f46d5-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f46d5-114">Request body</span></span>
<span data-ttu-id="f46d5-115">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="f46d5-115">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f46d5-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="f46d5-116">Response</span></span>

<span data-ttu-id="f46d5-117">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f46d5-117">If successful, this method returns `201, Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f46d5-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f46d5-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f46d5-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f46d5-119">Request</span></span>
<span data-ttu-id="f46d5-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f46d5-120">Here is an example of the request.</span></span>
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
<span data-ttu-id="f46d5-121">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="f46d5-121">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f46d5-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="f46d5-122">Response</span></span>
<span data-ttu-id="f46d5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f46d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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