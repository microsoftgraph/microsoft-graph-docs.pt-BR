# <a name="update-a-group-setting"></a><span data-ttu-id="db127-101">Atualizar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="db127-101">Update a group setting</span></span>

<span data-ttu-id="db127-102">Atualize as propriedades de um objeto de configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="db127-102">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db127-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="db127-103">Permissions</span></span>

<span data-ttu-id="db127-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="db127-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="db127-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db127-106">Permission type</span></span>      | <span data-ttu-id="db127-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db127-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db127-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db127-108">Delegated (work or school account)</span></span> | <span data-ttu-id="db127-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db127-109">Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db127-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db127-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db127-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db127-111">Not supported.</span></span>    |
|<span data-ttu-id="db127-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db127-112">Application</span></span> | <span data-ttu-id="db127-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db127-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db127-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db127-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="db127-115">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="db127-115">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="db127-116">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="db127-116">Optional request headers</span></span>
| <span data-ttu-id="db127-117">Nome</span><span class="sxs-lookup"><span data-stu-id="db127-117">Name</span></span> | <span data-ttu-id="db127-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="db127-118">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="db127-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="db127-119">Authorization</span></span>  | <span data-ttu-id="db127-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db127-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db127-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db127-122">Content-Type</span></span>  | <span data-ttu-id="db127-123">application/json</span><span class="sxs-lookup"><span data-stu-id="db127-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="db127-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db127-124">Request body</span></span>
<span data-ttu-id="db127-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="db127-125">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="db127-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db127-126">Property</span></span> | <span data-ttu-id="db127-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="db127-127">Type</span></span> | <span data-ttu-id="db127-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="db127-128">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="db127-129">values</span><span class="sxs-lookup"><span data-stu-id="db127-129">values</span></span> | <span data-ttu-id="db127-130">settingValue</span><span class="sxs-lookup"><span data-stu-id="db127-130">settingValue</span></span> | <span data-ttu-id="db127-p103">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="db127-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="db127-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="db127-134">Response</span></span>

<span data-ttu-id="db127-135">Se bem-sucedido, este método retorna o código de resposta `204 OK` e o objeto [groupSetting](../resources/groupsetting.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db127-135">If successful, this method returns a `204 OK` response code and updated [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db127-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db127-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db127-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db127-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="db127-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="db127-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->