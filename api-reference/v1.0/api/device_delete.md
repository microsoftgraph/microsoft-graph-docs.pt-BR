# <a name="delete-device"></a><span data-ttu-id="560c7-101">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="560c7-101">Delete device</span></span>

<span data-ttu-id="560c7-102">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="560c7-102">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="560c7-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="560c7-103">Permissions</span></span>
<span data-ttu-id="560c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="560c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="560c7-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="560c7-106">Permission type</span></span>      | <span data-ttu-id="560c7-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="560c7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="560c7-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="560c7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="560c7-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="560c7-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="560c7-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="560c7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="560c7-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="560c7-111">Not supported.</span></span>    |
|<span data-ttu-id="560c7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="560c7-112">Application</span></span> | <span data-ttu-id="560c7-113">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="560c7-113">Device.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="560c7-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="560c7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="560c7-115">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="560c7-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="560c7-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="560c7-116">Request headers</span></span>
| <span data-ttu-id="560c7-117">Nome</span><span class="sxs-lookup"><span data-stu-id="560c7-117">Name</span></span>       | <span data-ttu-id="560c7-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="560c7-118">Type</span></span> | <span data-ttu-id="560c7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="560c7-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="560c7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="560c7-120">Authorization</span></span>  | <span data-ttu-id="560c7-121">string</span><span class="sxs-lookup"><span data-stu-id="560c7-121">string</span></span>  | <span data-ttu-id="560c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="560c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="560c7-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="560c7-124">Request body</span></span>
<span data-ttu-id="560c7-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="560c7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="560c7-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="560c7-126">Response</span></span>

<span data-ttu-id="560c7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="560c7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="560c7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="560c7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="560c7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="560c7-130">Request</span></span>
<span data-ttu-id="560c7-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="560c7-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="560c7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="560c7-132">Response</span></span>
<span data-ttu-id="560c7-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="560c7-133">Here is an example of the response.</span></span>
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
