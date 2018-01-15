# <a name="delete-device"></a><span data-ttu-id="1210d-101">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="1210d-101">Delete device</span></span>

<span data-ttu-id="1210d-102">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="1210d-102">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="1210d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="1210d-103">Permissions</span></span>
<span data-ttu-id="1210d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1210d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="1210d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1210d-106">Permission type</span></span>      | <span data-ttu-id="1210d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1210d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1210d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1210d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1210d-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1210d-109">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1210d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1210d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1210d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1210d-111">Not supported.</span></span>    |
|<span data-ttu-id="1210d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1210d-112">Application</span></span> | <span data-ttu-id="1210d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1210d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1210d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1210d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="1210d-115">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="1210d-115">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1210d-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1210d-116">Request headers</span></span>
| <span data-ttu-id="1210d-117">Nome</span><span class="sxs-lookup"><span data-stu-id="1210d-117">Name</span></span>       | <span data-ttu-id="1210d-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1210d-118">Type</span></span> | <span data-ttu-id="1210d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1210d-119">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1210d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1210d-120">Authorization</span></span>  | <span data-ttu-id="1210d-121">string</span><span class="sxs-lookup"><span data-stu-id="1210d-121">string</span></span>  | <span data-ttu-id="1210d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1210d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1210d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1210d-124">Request body</span></span>
<span data-ttu-id="1210d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1210d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1210d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1210d-126">Response</span></span>

<span data-ttu-id="1210d-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1210d-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1210d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1210d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1210d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1210d-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="1210d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1210d-131">Response</span></span>

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
