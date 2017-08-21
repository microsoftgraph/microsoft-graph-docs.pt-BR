# <a name="create-registeredowner"></a><span data-ttu-id="f8e34-101">Criar registeredOwner</span><span class="sxs-lookup"><span data-stu-id="f8e34-101">Create registeredOwner</span></span>

<span data-ttu-id="f8e34-102">Adiciona um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8e34-102">Add a user as a registered owner of the device.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8e34-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8e34-103">Prerequisites</span></span>
<span data-ttu-id="f8e34-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="f8e34-104">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="f8e34-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8e34-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/registeredOwners

```
## <a name="request-headers"></a><span data-ttu-id="f8e34-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e34-106">Request headers</span></span>
| <span data-ttu-id="f8e34-107">Nome</span><span class="sxs-lookup"><span data-stu-id="f8e34-107">Name</span></span>       | <span data-ttu-id="f8e34-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8e34-108">Type</span></span> | <span data-ttu-id="f8e34-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8e34-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f8e34-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8e34-110">Authorization</span></span>  | <span data-ttu-id="f8e34-111">string</span><span class="sxs-lookup"><span data-stu-id="f8e34-111">string</span></span>  | <span data-ttu-id="f8e34-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8e34-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8e34-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e34-114">Request body</span></span>
<span data-ttu-id="f8e34-115">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="f8e34-115">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f8e34-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8e34-116">Response</span></span>

<span data-ttu-id="f8e34-117">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8e34-117">If successful, this method returns `201, Created` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8e34-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8e34-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8e34-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8e34-119">Request</span></span>
<span data-ttu-id="f8e34-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8e34-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_device"
}-->
```http
POST https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
Content-type: application/json
Content-length: 30

{
  "directoryObject": {
  }
}
```
<span data-ttu-id="f8e34-121">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="f8e34-121">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f8e34-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8e34-122">Response</span></span>
<span data-ttu-id="f8e34-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8e34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create registeredOwner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->