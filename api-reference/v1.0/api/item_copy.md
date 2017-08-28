# <a name="copy-a-driveitem"></a><span data-ttu-id="258aa-101">Copiar um DriveItem</span><span class="sxs-lookup"><span data-stu-id="258aa-101">Copy a DriveItem</span></span>

<span data-ttu-id="258aa-102">Cria uma cópia de um [driveItem](../resources/driveitem.md) (incluindo todos os filhos) em um novo pai ou com um novo nome.</span><span class="sxs-lookup"><span data-stu-id="258aa-102">Creates a copy of a [driveItem](../resources/driveitem.md) (including any children) under a new parent or with a new name.</span></span>

## <a name="permissions"></a><span data-ttu-id="258aa-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="258aa-103">Permissions</span></span>
<span data-ttu-id="258aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="258aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="258aa-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="258aa-106">Permission type</span></span>      | <span data-ttu-id="258aa-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="258aa-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="258aa-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="258aa-108">Delegated (work or school account)</span></span> | <span data-ttu-id="258aa-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="258aa-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="258aa-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="258aa-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="258aa-111">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="258aa-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="258aa-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="258aa-112">Application</span></span> | <span data-ttu-id="258aa-113">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="258aa-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="258aa-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="258aa-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
POST /me/drive/items/{item-id}/copy
POST /me/drive/root:/{path}:/copy
POST /groups/{group-id}/drive/items/{item-id}/copy
```

## <a name="request-body"></a><span data-ttu-id="258aa-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="258aa-115">Request body</span></span>
<span data-ttu-id="258aa-116">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="258aa-116">In the request body, provide a JSON object with the following parameters.</span></span>


| <span data-ttu-id="258aa-117">Nome</span><span class="sxs-lookup"><span data-stu-id="258aa-117">Name</span></span>            | <span data-ttu-id="258aa-118">Valor</span><span class="sxs-lookup"><span data-stu-id="258aa-118">Value</span></span>                                          | <span data-ttu-id="258aa-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="258aa-119">Description</span></span>                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="258aa-120">parentReference</span><span class="sxs-lookup"><span data-stu-id="258aa-120">parentReference</span></span> | [<span data-ttu-id="258aa-121">ItemReference</span><span class="sxs-lookup"><span data-stu-id="258aa-121">ItemReference</span></span>](../resources/itemreference.md) | <span data-ttu-id="258aa-p102">Opcional. Referência ao item pai em que a cópia será criada.</span><span class="sxs-lookup"><span data-stu-id="258aa-p102">Optional. Reference to the parent item the copy will be created in.</span></span>                                         |
| <span data-ttu-id="258aa-124">name</span><span class="sxs-lookup"><span data-stu-id="258aa-124">name</span></span>            | <span data-ttu-id="258aa-125">string</span><span class="sxs-lookup"><span data-stu-id="258aa-125">string</span></span>                                         | <span data-ttu-id="258aa-p103">Opcional. O novo nome para a cópia. Se isso não for fornecido, será usado o mesmo nome que o original.</span><span class="sxs-lookup"><span data-stu-id="258aa-p103">Optional. The new name for the copy. If this isn't provided, the same name will be used as the original.</span></span>    |

<span data-ttu-id="258aa-p104">**Observação:** _parentReference_ deve incluir um `id` ou `path` mas não ambos. Se ambos forem incluídos, precisarão fazer referência ao mesmo item ou ocorrerá um erro.</span><span class="sxs-lookup"><span data-stu-id="258aa-p104">**Note:** The _parentReference_ should include either an `id` or `path` but not both. If both are included, they need to reference the same item or an error will occur.</span></span>

## <a name="example"></a><span data-ttu-id="258aa-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="258aa-131">Example</span></span>

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "contoso plan.docx"
}
```

## <a name="response"></a><span data-ttu-id="258aa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="258aa-132">Response</span></span>

<span data-ttu-id="258aa-133">Retorna detalhes sobre como monitorar o progresso da cópia após aceitar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="258aa-133">Returns details about how to monitor the progress of the copy, upon accepting the request.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
```

## <a name="remarks"></a><span data-ttu-id="258aa-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="258aa-134">Remarks</span></span>

<span data-ttu-id="258aa-p105">Em muitos casos, a ação de copiar é executada de forma assíncrona. A resposta da API só indicará que a operação de cópia foi aceita ou rejeitada, por exemplo, porque o nome de arquivo de destino já está sendo utilizado.</span><span class="sxs-lookup"><span data-stu-id="258aa-p105">In many cases the copy action is performed asynchronously. The response from the API will only indicate that the copy operation was accepted or rejected, say due to the destination filename already being in use.</span></span>

<span data-ttu-id="258aa-137">**Observação:** A API não fornece um método para saber se a cópia foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="258aa-137">**Note:** The API does not provide a method to know if the copy was successful.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Copy"
} -->
