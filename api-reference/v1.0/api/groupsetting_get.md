# <a name="get-a-group-setting"></a><span data-ttu-id="30088-101">Obtenha uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="30088-101">Get a group setting</span></span>

<span data-ttu-id="30088-102">Recupere as propriedades de um determinado objeto de configuração de grupo.</span><span class="sxs-lookup"><span data-stu-id="30088-102">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="30088-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="30088-103">Permissions</span></span>

<span data-ttu-id="30088-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="30088-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="30088-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30088-106">Permission type</span></span>      | <span data-ttu-id="30088-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30088-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30088-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30088-108">Delegated (work or school account)</span></span> | <span data-ttu-id="30088-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="30088-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="30088-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30088-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30088-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30088-111">Not supported.</span></span>    |
|<span data-ttu-id="30088-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30088-112">Application</span></span> | <span data-ttu-id="30088-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30088-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30088-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30088-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="30088-115">Obter uma configuração de todo o locatário ou específico.</span><span class="sxs-lookup"><span data-stu-id="30088-115">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30088-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30088-116">Optional query parameters</span></span>
<span data-ttu-id="30088-117">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30088-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="30088-118">Observação: $filter não é suportado.</span><span class="sxs-lookup"><span data-stu-id="30088-118">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30088-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30088-119">Request headers</span></span>
| <span data-ttu-id="30088-120">Nome</span><span class="sxs-lookup"><span data-stu-id="30088-120">Name</span></span> | <span data-ttu-id="30088-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="30088-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="30088-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="30088-122">Authorization</span></span> | <span data-ttu-id="30088-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30088-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30088-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30088-125">Request body</span></span>

<span data-ttu-id="30088-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30088-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30088-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="30088-127">Response</span></span>

<span data-ttu-id="30088-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30088-128">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30088-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30088-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30088-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30088-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="30088-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="30088-131">Response</span></span>

<span data-ttu-id="30088-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30088-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->