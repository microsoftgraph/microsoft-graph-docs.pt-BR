# <a name="delete-device"></a><span data-ttu-id="e14cc-101">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="e14cc-101">Delete device</span></span>

<span data-ttu-id="e14cc-102">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="e14cc-102">Delete a registered device.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e14cc-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e14cc-103">Prerequisites</span></span>
<span data-ttu-id="e14cc-104">Um dos seguintes **escopos** é necessário para executar esta API: *Directory.AccessAsUser.All* ou *Device.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="e14cc-104">One of the following **scopes** is required to execute this API: *Directory.AccessAsUser.All*, *Device.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="e14cc-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e14cc-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="e14cc-106">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="e14cc-106">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e14cc-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e14cc-107">Request headers</span></span>
| <span data-ttu-id="e14cc-108">Nome</span><span class="sxs-lookup"><span data-stu-id="e14cc-108">Name</span></span>       | <span data-ttu-id="e14cc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e14cc-109">Type</span></span> | <span data-ttu-id="e14cc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e14cc-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e14cc-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="e14cc-111">Authorization</span></span>  | <span data-ttu-id="e14cc-112">string</span><span class="sxs-lookup"><span data-stu-id="e14cc-112">string</span></span>  | <span data-ttu-id="e14cc-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e14cc-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e14cc-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e14cc-115">Request body</span></span>
<span data-ttu-id="e14cc-116">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e14cc-116">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e14cc-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="e14cc-117">Response</span></span>

<span data-ttu-id="e14cc-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e14cc-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e14cc-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e14cc-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e14cc-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e14cc-121">Request</span></span>
<span data-ttu-id="e14cc-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e14cc-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="e14cc-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="e14cc-123">Response</span></span>
<span data-ttu-id="e14cc-124">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e14cc-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
